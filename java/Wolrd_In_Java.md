---
title: Wolrd In Java
date: 2018-10-28
categories: ["java"]
tags: ["java"]
---


# 深入理解Java

有空就记录一点小内容！！

## Java接口与抽象类的区别

Java提供和支持创建抽象类和接口。它们的实现有共同点，不同点在于：

1. 接口中所有的方法隐含的都是抽象的。而抽象类则可以同时包含抽象和非抽象的方法。
2. 类可以实现很多个接口，但是只能继承一个抽象类
3. 类可以不实现抽象类和接口声明的所有方法，当然，在这种情况下，类也必须得声明成是抽象的。
4. 抽象类可以在不提供接口方法实现的情况下实现接口。
5. Java接口中声明的变量默认都是final的。抽象类可以包含非final的变量。
6. Java接口中的成员函数默认是**public**的。抽象类的成员函数可以是private，protected或者是public。
7. **接口是绝对抽象的，不可以被实例化，抽象类也不可以被实例化**。
8. 一个类实现接口的话要实现接口的所有方法，而抽象类不一定

一句话总结：
<!-- more -->
**从设计层面来说，抽象是对类的抽象，是一种<font color="red">模板设计</font>，接口是行为的抽象，是一种行为的规范**



## **浅克隆和深克隆** 

​	 Java语言中，数据类型分为值类型（基本数据类型）和引用类型.

- **值类型**包括int、double、byte、boolean、char等简单数据类型，

- **引用类型**包括类、接口、数组等复杂类型。

浅克隆和深克隆的主要区别在于是否支持引用类型的成员变量的复制，下面将对两者进行详细介绍。 

**浅克隆**(ShallowClone)

  在浅克隆中，如果原型对象的成员变量是**值类型**，将复制一份给克隆对象；如果原型对象的成员变量是**引用类**型，则将**引用对象的地址**复制一份给克隆对象，也就是说原型对象和克隆对象的成员变量指向相同的内存地址。简单来说，在浅克隆中，当对象被复制时只复制它本身和其中包含的值类型的成员变量，而引用类型的成员对象并没有复制。

**深克隆**(DeepClone)

在深克隆中，无论原型对象的成员变量是值类型还是引用类型，都将复制一份给克隆对象，深克隆将原型对象的所有引用对象也复制一份给克隆对象。简单来说，在深克隆中，除了对象本身被复制外，对象所包含的所有成员变量也将复制。





