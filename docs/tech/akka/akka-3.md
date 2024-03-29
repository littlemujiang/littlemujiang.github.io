# 3.Actor进阶：创建带参数的actor和发送复杂的消息类型


上一篇实现了actor的创建，但是这个actor并不能满足我们生产中的要求。主要有以下2点：

1. 构建actor类时，需要带参数或配置
2. 消息不会是String这种基本类型，会是一个自定义的类

针对上面的问题，我们扩展之前的HelloWorldActor，并引入akka的一些用法或思想。

<p id = "build"></p>
---

[TOC]

## 定义带参数的actor

构建带参数的actor的方法，可以通过actor类的create()静态方法，传递到私有化的构造方法中，再在构造方法中赋值到actor类的内部变量就可以了。如下所示：


```java
@Slf4j
public class FilterActor extends AbstractBehavior<IDeviceMessage> {

    private BehaviorConfig config;
    private ActorRef nextActorRef;

    private FilterActor(ActorContext<IDeviceMessage> context, BehaviorConfig behaviorConfig, ActorRef nextActor) {
        super(context);
        this.config = behaviorConfig;
        this.nextActorRef = nextActor;
    }

    //传2个参数，一个是自定义的配置类，一个是连接的下一个actor
    public static Behavior<IDeviceMessage> create(BehaviorConfig behaviorConfig, ActorRef nextActor) {
        return Behaviors.setup(context ->  new FilterActor(context, behaviorConfig, nextActor)
        );
    }

}
```

其中`BehaviorConfig`是我们自定义的配置类。创建actor实例的时候传入create()方法中，如下所示：


```java
    // actor的配置
    BehaviorConfig filterConfig = new BehaviorConfig("$power > 2000");
    // 创建filter的behavior
    Behavior<IDeviceMessage> filterBehavior = FilterActor.create(filterConfig, null);
    // 实例化filter actor
    ActorRef<IDeviceMessage> filterActorRef = context.spawn(filterBehavior, "Filter");
```


## 自定义消息类型

我们通常要处理的数据/消息一般不会是基本类型，通常是我们自己定义的pojo类，而且也通常不会是同一种类型的消息，会处理多种类型的消息。
下面我们把上面例子里的消息类型改造成自定义的消息类型。

在改造之前，需要说明，在akka的规范中，一个actor只能接收并处理某一类的消息类型。也就是说在实现上，这些消息需要实现自同一个接口类。可以理解为，这个actor并不是什么都能拿来加工。比如说这个actor就是个木工，那只能接收各种木头进行加工，黑檀木、桃木、松木都可以，但是来块铁板就不行了。

因此，我们需要先定义一个基础消息接口，这个接口可以什么都没有，但这是常规操作。

```java
public interface IDeviceMessage {
}
```

然后定义表示设备属性的消息类，其中包含电流、电压、功率等属性。

```java
@Data
@Builder
public class DevicePropertyMessage implements IDeviceMessage {
    private int msgId;
    private String thingId;
    private double current;
    private double voltage;
    private double power;
}
```

定义完消息类后，需要修改Actor的定义，主要是修改Behavior、ActorContext、Receive后面泛型里的类，需要修改为上面定义的接口类。比如：


```java
    //返回的Behavior限定了此actor可处理的消息类型
    public static Behavior<IDeviceMessage> create(BehaviorConfig behaviorConfig, ActorRef<IDeviceMessage> nextActor) {
        return Behaviors.setup(context ->  new FilterActor(context, behaviorConfig, nextActor));
    }
```

然后，在`createReceive()`方法中指定不同消息的处理方法。


```java
    @Override
    public Receive<IDeviceMessage> createReceive() {
        return newReceiveBuilder()
                //不同类型的消息，指定不同的方法处理
                .onMessage(DevicePropertyMessage.class, this::onPropertyMessage)
                .onMessage(DeviceActionMessage.class, this::onActionMessage)
                .build();
    }
```


以上，我们实现了一个更实用的actor，可以接收自定义的消息类型，并按我们的配置的逻辑进行处理。
