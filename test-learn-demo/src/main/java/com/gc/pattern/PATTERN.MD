### 设计模式七大原则
- 1.开闭原则:对拓展开发,对修改关闭
- 2.职责单一原则:每个方法,接口,类负责单一职责
- 3.接口隔离原则:一个类对类的依赖应该建立在最小的接口之上;客户端不应该依赖它不需要的接口.
- 4.依赖倒置原则:面向接口编程.
- 5.迪米特法则:一个对象应该对其他对象保持最少的了解,又叫最少知道原则.
- 6.合成复用原则:少用继承,尽量多使用组合(has-a)/聚合(contains-a)
- 7.里式替换原则:子类可以拓展父类的功能,但是不能覆盖父类原有的功能.


### 设计模式中英对照表
| Chinese          		| English   						|  定义	|
| :----:   			| :----:  							| :----:|
|1.工厂方法模式			|Factory Method Pattern				| |
|2.抽象工厂模式			|Abstract Factory Pattern   		| |
|3.建造者模式			|Builder Pattern            		| |
|4.原型模式				|Prototype Pattern          		| |
|5.单例模式				|Singleton Pattern          		||
|6.适配器模式			|Adapter Pattern            		||
|7.桥梁模式/桥接模式	    |Bridge Pattern         			||
|8.组合模式				|Composite Pattern          		||
|9.装饰模式				Decorator Pattern           		||
|10.门面模式/外观模式	    |Facade Pattern         			||
|11.享元模式			    |Flyweight Pattern					||
|12.代理模式			    |Proxy pattern          			||
|13.责任链模式			|Chain of Responsibility Pattern	||
|14.命令模式	            |Command Pattern					||
|15.解释器模式			|Interpreter Pattern				||
|16.迭代器模式			|Iterator Pattern					||
|17.中介者模式			|Mediator Pattern					||
|18.备忘录模式			|Memento Pattern 					||
|19.观察者模式			|Observer Pattern					||
|20.状态模式			    |State Pattern   					||
|21.策略模式			    |Strategy Pattern					||
|22.模板方法模式		    |Template Method Pattern			||
|23.访问者模式			|Visitor Pattern					||

### 设计模式的分类
|分类|设计模式|备注|
|----|----|----|
|创建型|原型模式(Prototype),单例模式(Singleton),工厂方法模式(Factory Method),抽象工厂模式(Abstract Factory),建造者模式(Builder)|`简单工厂(Simple Factory)不属于GOF23种设计模式`|
|结构型|适配器模式(Adapter),装饰者模式(Decorator),代理模式(Proxy),桥接模式(Bridge),组合模式(Composite),门面模式(Facade),享元模式(Flyweight)||
|行为型|观察者模式(Observer),模板方法模式(Template Method),策略模式(Strategy),解释器模式(Interpreter),责任链模式(Chain of Responsibility),命令模式(Command),迭代器模式(Iterator),调解者模式(Mediator),备忘录模式(Memento),状态模式(State)|`委派模式(Delegate)不属于GOF23种设计模式`|

注意:
> `图片请参考 设计模式图片.png`

### 设计模式之间的关联和对比
**单例模式和工厂模式**
实际业务代码中,通常会把工厂类设计为单例

**策略模式和工厂模式**
- 工厂模式包含工厂方法模式和抽象工厂模式是创建型模式;策略模式属于行为型模式
- 工厂模式主要目的是封装好创建逻辑,策略模式接收工厂创建好的对象,从而实现不同的行为.

**策略模式和委派模式**
1. 策略模式是委派模式内部的一种实现形式,策略模式关注的结果是否能互相替代;
2. 委派模式更关注分发和调度的过程;不属于GOF23种模式.

**模板方法模式和工厂方法模式**
工厂方法是模板方法的一种特殊实现.对于工厂方法而言,相当于只有一个步骤的模板方法模式.这个步骤交给子类去实现;对于模板方法而言,将一个或者多个步骤交给子类实现,但是并不会改变父类算法的结构.

**模板方法模式和策略模式**
1. 模板方法和策略都有封装算法
2. 模板方法模式是针对定义一个算法的流程,将一个或者多个步骤交给子类实现;策略模式针是使不同算法可以相互替换,且不影响客户端应用层的使用
3. 模板方法不能改变算法结构,策略模式可以改变算法结构且可以替换.策略模式通常用来代替if...else...等条件分支语句,让你的代码更加简洁

**装饰器模式和静态代理模式**
1. 装饰者更注重的是对象的功能拓展;静态代理注重的是对象的访问控制,解耦
2. 装饰者把被装饰者作为构造参数;静态代理会在代理类中创建被代理对象的实例.

`装饰者和静态代理虽然都持有对方引用,但是处理的重心是不一样的`

***装饰者模式和适配器模式***
1. 装饰者模式和适配器模式都属于包装器模式(Wrapper Pattern)
2. 装饰者模式可以实现和被装饰者相同的接口(相同的父类)或者继承被装饰者做为它的子类.而适配器和被适配者可以实现不同的接口
3. 装饰者模式是前置考虑,更多的是为了类的功能拓展;而适配器是后置考虑,更加的注重兼容和转换

***适配器和静态代理模式***
适配器可以结合静态代理来实现,保存被适配对象的引用,但不是唯一的实现方式。

***适配器和策略模式***
在适配业务复杂的情况下,利用策略模式优化动态适配逻辑




### Spring中常用的设计模式对比

### Spring中编程思想总结
































