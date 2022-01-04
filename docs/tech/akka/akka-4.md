# 4.Actor间的交互与停止


> “actor之间需要协作才能完成各项功能，协作需要沟通”

<p id = "build"></p>
---

[TOC]


##  Actor间的交互

在实际场景中，我们需要很多类型的actor协助来完成一项任务或功能。这就涉及actor建的交互。actor最基本也是最常用的方式就是`actorRef.tell(message)`。 这个方法是异步的，akka非阻塞的优势也正是通过这一点体现出来的。

* **注**：使用tell()有2个前提，要获取被tell的actor的ActorRef，以及此actor能接收的消息的类型。

实际场景中，可能会有其他场景，比如需要返回处理的结果、或者定时给自己发消息，可以参考akka的文档：

[akka官方文档：actor交互模式](https://doc.akka.io/docs/akka/current/typed/interaction-patterns.html)



##  Actor的停止

某些场景下，actor可能会被不再使用，那我们需要将其停止并释放资源。在之前的classic版本中，给这个actor发一个`PoisonPill`消息就能停止这个actor，在typed版本下，则需要我们自己实现。也比较简单，只要配置stop消息的处理方法，并在方法中返回`Behaviors.stopped()`即可。



```java
    @Override
    public Receive<IDeviceMessage> createReceive() {
        return newReceiveBuilder()
                //不同类型的消息，指定不同的方法处理
                .onMessage(DevicePropertyMessage.class, this::onPropertyMessage)
                .onMessage(DeviceActionMessage.class, this::onActionMessage)
                //接收停止actor的消息
                .onMessage(StopMessage.class, this::onStopMessage)
                //actor停止后的回调方法
                .onSignal(PostStop.class, this::onPostStop)
                .build();
    }
```


```java
    private Behavior<IDeviceMessage> onStopMessage(StopMessage msg) {
        log.info("[filter actor] stopped" );
        return Behaviors.stopped();
    }
```

这里的`return Behaviors.stopped()`表示在收到StopMessage类型的消息后，将actor的行为模式转变为Behaviors.stopped()，即停止状态。


如果actor内有需要主动释放的资源，可以通过`onSignal()`接收`PostStop.class`的信号，并在指定的方法内进行处理。

