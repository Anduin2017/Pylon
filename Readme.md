# Aiursoft Pylon

> 星灵（Protoss）依靠Khaydarin水晶进行灵能链接。所有星灵依靠灵能链接维系社会秩序（不包括黑暗圣堂武士，他们切断了自己的神经束），这种秩序被叫做卡拉之道。而水晶塔（Pylon）则是真正将这些幽能输送给不同地区所必须的设施，每座水晶塔都可以散发出一种短距离的能量，提供给附近的能源和折跃门来使用。

水晶塔是Protoss所有建筑的基础，除Assimilators和Nexus外。

## Pylon的位置

在Aiursoft中，Pylon是所有Aiursoft高层应用的基础。任何Aiursoft高层应用必须依赖Pylon。

比较有趣的是，Nexus项目本身并不依赖Pylon。这也是Aiursoft对星灵的设计结构的尊重。

## Pylon中的代码包含什么

在Pylon的代码中，主要包含两个部分：

* 对Aiursoft的API的抽象
* Aiursoft高层应用常用的基础方法

## 为什么要有Pylon

在Pylon的基础上，Aiursoft的底层基础设施和高层服务都将对Pylon的抽象进行实现。在此设计基础上，在开发任何Aiursoft高层应用时，可以直接依赖Pylon来快速接入Aiursoft API。或未来需要调整底层实现时，使用新的代码来实现Pylon中的抽象，而对于高层业务来说是无感知的。

另外，Pylon中共享了大量Aiursoft常用的基类方法和扩展方法，来帮助使ASP.NET Core的Web应用开发变得更加简单方便。

## 这个项目适合我吗

更多情况下，不。不适合。它是为Aiursoft构建的。

但是，Pylon中有众多好用的扩展方法，或许对于其它ASP.NET Core的应用来说非常实用。包括：

* HTTP请求库
* 强类型URL格式化器
* IP地址请求熔断器
* 对象示例实例化器
* API文档生成器
* string扩展操作库
* 计数器
* RSA签名、加密操作库

如果你真的专注于Aiursoft的扩展开发、开发Aiursoft的高层应用、研究Aiursoft的底层基础设施的实现，Pylon不失为一个不错的案例。

## Pylon的版本历史

请参考：[Nuget](https://www.nuget.org/packages/Aiursoft.Pylon/)
