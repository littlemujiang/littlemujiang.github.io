# 4 自定义应用服务（python）

很多时候，我们不能基于go去开发与edgex整合或联动的application service。
比如需要调用算法模型对数据进行计算，那用python编写application service更合适些。
这样便不能使用edgex SDK提供的messagebus了。好在edgex默认使用了redis pipeline作为消息通道。我们可以直接连接redis，从redis中取出event进行处理。


## 从pipeline接收数据

接收数据比较简单，连接上redis后，开启一个订阅，然后处理消息即可。

需要注意的是，redis pipeline中的topic层级是用点分割的，而edgex配置文件中的斜杠分割，是会在代码中进行替换的。并且通配符也要由#变为*。
示例如下：`edgex.events.device.*`， `edgex.events.device.{device-profile-name}.{device-name}.{source-name}`



## 处理数据

比较麻烦的是对消息的处理，我们从redis pipeline接收到的是被层层包装过的字节流，而我们需要的其实是里面的event。

我们从redis中收到的最原始的数据如下：

```
[b'pmessage', b'edgex.events.device.*', b'edgex.events.device.gbKkLslQ.5e9cabad3b5.collected', b'{"ReceivedTopic": "", "CorrelationID": "", "Payload": "eyJhcGlWZXJzaW9u……I6IG9hdDY0In1dfX0=", "ContentType": "application/json"}']
```

是一个数组。其中第2项是我们订阅的带通配符的topic，第3项是具体的topic，第4项中包含数据，具体在Payload中。

Payload是一串非明文的码，默认是经过base64算法encode过的数据（edgex支持使用加密算法加密后再base64，暂时没研究）。因此我们需要使用base64算法decode，转换后并转化为json后的明文如下：

```json
{
    "apiVersion":"v2",
    "requestId":"aa349b4b-8d2b-445f-81ed-c02a7724624a",
    "event":{
        "apiVersion":"v2",
        "id":"2f9883e9-dd33-45e1-a8c9-3c4d529afdbc",
        "profileName":"gbKkLslQ",
        "deviceName":"5e9ca055b72f4275b6bc0c425fbad3b5",
        "sourceName":"product_data",
        "origin":1648536800443000000,
        "readings":[
            {
                "id":null,  //直接模拟的数据，部分有缺失
                "profileName":"gbKkLslQ",
                "deviceName":"5e9ca055b72f4275b6bc0c425fbad3b5",
                "resourceName":"Inletflow",
                "origin":1648536800443000000,
                "value":"98.3487176418304",
                "valueType":"Float64"
            }
        ]
    }
}
```

现在可以看到里面是我们需要的event数据。然后就可以取出里面的数据处理了。



## 发送消息回pipeline

有些场景是，我们用几个属性的数据，通过调用算法模型计算另一个属性的值，这时我们还要把计算结果发回redis pipeline，这样才方便让消息流入规则引擎（edgex-kuiper），继续进行处理。

这种情况就需要按解码的过程，倒着进行编码。也就是说，要把计算出的值先放入reading，再封装成event，再base64编码成Payload，再构造成原始消息的数组。
并且发送给redis的topic也要用 `edgex.events.device.{device-profile-name}.{device-name}.{source-name}`这种结构。

这样，便完成了从pipeline收消息，处理，再发回pipeline的闭环。