# Java-Virtual-Machine

Java虚拟机资源汇总

## 最后更新时间

2019-10-24

## 注意

1. 资料的排列的顺序不分先后。
2. 资料的所有权归原作者所有，这里是汇总。
3. 知识水平的限制，导致资料的介绍或者范围有一定的局限性，欢迎指出。

## 8. JVM 3000问

### 1. 为何从Java8开始，Permanent区域被取消变成了Metaspace区域
>

> 该文介绍了HotSpotVM的Permanent(永久代)变化为Metaspace(元数据)的原因和影响，文章是日文的，近期可能会翻译成中文

+ [Java8的HotSpotVM的Permanent领域替换为MetaSpace领域的理由和影响](http://equj65.net/tech/java8hotspot/)

### 2. 先有Class还是先有Object
>

> 源自知乎的一个问题，对于Java来说，所有类的父类都是Object类，但是Object类本身又属于类类型，即Class类型，那么问题就来了。

+ [先有Class还是先有Object？](https://www.zhihu.com/question/30301819)

### 3. JVM简史
>

> 源自周老师的文章，讲述了JVM虚拟机的发展史，以及各种各样的Java虚拟机

+ [Java虚拟机家族考](https://www.infoq.cn/article/jvm-family)

### 4. lambda表达式的实现原理
>

> 作者:让猪再飞会

> 虽然Java12都出来了，但是对于lambda表达式的实现原理以及用法你或许还是一知半解，可以阅读以下这篇文章，会有收获。

+ [Lambda表达式](http://www.cnblogs.com/WJ5888/p/4618465.html)
+ [Lambda实现原理分析](https://www.cnblogs.com/WJ5888/p/4667086.html)

### 5. Invokedynamic Java的秘密武器
>

> 来自infoq的翻译文章，主要是讲述了InvokeDynamic指令所起到的作用。

+ [Invokedynamic Java的秘密武器](https://www.infoq.cn/article/Invokedynamic-Javas-secret-weapon)

### 6. Java到底是值传递还是引用传递
>

> 作者:假不理

> 作者从问题的源头出发详细的分析了Java为何是值传递这一问题。

+ [Java为何是值传递](https://juejin.im/post/5bce68226fb9a05ce46a0476)

## 9. Java 虚拟机规范

虚拟机规范，对Java虚拟机的抽象实现作了一定的规定和描述，但并没有规定具体的实现方式，虚拟机的厂商只要遵守了规范的规定，实现方式是可以自由选择的。
规范可以作为工具类书籍随时查看，虽然现在Java已经更新到12了，但是其实虚拟机的规范变化不是很大。读者们仍然可以参照周先生翻译的Java SE 8 或者 Java SE 7 规范。

### Java 虚拟机规范英文版

> 资料类型：HTML,PDF
>
> 版本：Second Edition~ Java SE 11 Edition

+ [The Java® Virtual Machine Specification](https://docs.oracle.com/javase/specs/index.html)

### Java 虚拟机规范中文版

> 资料类型：书籍,PDF
>
> 作者：周志明 等

+ 《Java虚拟机规范（Java SE 7版）》
+ 《Java虚拟机规范（Java SE 8版）》

## 10. 文章系列

### 10.1 手写JVM系列

> 作者：[zachaxy](https://zachaxy.github.io/)
>

该系列从解析class文件开始，一步一步教读者如何去手动实现一个简单的玩具。文章思路清醒，排版优美。相关源代码可以参考原作者的github。

+ [手写JVM系列](https://zachaxy.github.io/tags/JVM/)
  + [手写JVM系列(1)-准备工作](https://zachaxy.github.io/2017/05/06/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-1-%E5%87%86%E5%A4%87%E5%B7%A5%E4%BD%9C/)
  + [手写JVM系列(2)-参数解析](https://zachaxy.github.io/2017/05/07/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-2-%E5%8F%82%E6%95%B0%E8%A7%A3%E6%9E%90/)
  + [手写JVM系列(3)-搜索class文件](https://zachaxy.github.io/2017/05/08/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-3-%E6%90%9C%E7%B4%A2class%E6%96%87%E4%BB%B6/)
  + [手写JVM系列(4)-分析class文件](https://zachaxy.github.io/2017/05/09/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-4-%E5%88%86%E6%9E%90class%E6%96%87%E4%BB%B6/)
  + [手写JVM系列(5)-分析class文件-常量池](https://zachaxy.github.io/2017/05/09/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-5-%E5%88%86%E6%9E%90class%E6%96%87%E4%BB%B6-%E5%B8%B8%E9%87%8F%E6%B1%A0/)
  + [手写JVM系列(6)-分析class文件-属性表](https://zachaxy.github.io/2017/05/09/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-6-%E5%88%86%E6%9E%90class%E6%96%87%E4%BB%B6-%E5%B1%9E%E6%80%A7%E8%A1%A8/)
  + [手写JVM系列(7)-读取class文件](https://zachaxy.github.io/2017/05/10/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-7-%E8%AF%BB%E5%8F%96class%E6%96%87%E4%BB%B6/)
  + [手写JVM系列(8)-运行时数据](https://zachaxy.github.io/2017/05/12/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-8-%E7%BA%BF%E7%A8%8B%E7%A7%81%E6%9C%89%E7%9A%84%E8%BF%90%E8%A1%8C%E6%97%B6%E6%95%B0%E6%8D%AE/)
  + [手写JVM系列(9)-指令集](https://zachaxy.github.io/2017/05/13/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-9-%E6%8C%87%E4%BB%A4%E9%9B%86/)  
  + [手写JVM系列(10)-解释器](https://zachaxy.github.io/2017/05/15/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-10%E8%A7%A3%E9%87%8A%E5%99%A8/)
  + [手写JVM系列(11)-线程共享的运行时数据](https://zachaxy.github.io/2018/01/03/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-11-%E7%BA%BF%E7%A8%8B%E5%85%B1%E4%BA%AB%E7%9A%84%E8%BF%90%E8%A1%8C%E6%97%B6%E6%95%B0%E6%8D%AE/)
  + [手写JVM系列(12)-类加载器的实现](https://zachaxy.github.io/2018/01/04/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-12-%E7%B1%BB%E5%8A%A0%E8%BD%BD%E5%99%A8%E7%9A%84%E5%AE%9E%E7%8E%B0/)
  + [手写JVM系列(13)-方法调用机制](https://zachaxy.github.io/2018/01/04/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-13-%E6%96%B9%E6%B3%95%E8%B0%83%E7%94%A8%E6%9C%BA%E5%88%B6/)
  + [手写JVM系列(14)-数组的实现](https://zachaxy.github.io/2018/01/12/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-14-%E6%95%B0%E7%BB%84%E7%9A%84%E5%AE%9E%E7%8E%B0/)  
  + [手写JVM系列(15)-字符串的实现](https://zachaxy.github.io/2018/01/16/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-15-%E5%AD%97%E7%AC%A6%E4%B8%B2%E7%9A%84%E5%AE%9E%E7%8E%B0/)
  + [手写JVM系列(16)-反射机制简介](https://zachaxy.github.io/2018/01/18/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-16-%E5%8F%8D%E5%B0%84%E6%9C%BA%E5%88%B6%E7%AE%80%E4%BB%8B/)
  + [手写JVM系列(17)-本地方法的调用过程](https://zachaxy.github.io/2018/01/18/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-17-%E6%9C%AC%E5%9C%B0%E6%96%B9%E6%B3%95%E7%9A%84%E8%B0%83%E7%94%A8%E8%BF%87%E7%A8%8B/)
  + [手写JVM系列(18)-异常处理机制](https://zachaxy.github.io/2018/01/20/%E6%89%8B%E5%86%99JVM%E7%B3%BB%E5%88%97-18-%E5%BC%82%E5%B8%B8%E5%A4%84%E7%90%86%E6%9C%BA%E5%88%B6/)  

### 10.2 Java虚拟机原理图解

> 作者：[亦山](https://blog.csdn.net/luanlouis)
>

作者通过大量的图例向读者们解释了虚拟机的部分原理，十分易懂。

+ [Java虚拟机原理图解](https://blog.csdn.net/column/details/jvm-principle.html)
  + [1. class 文件](####)(用来使排版美观一点:-))
    + [1.1 class文件基本组织结构](http://blog.csdn.net/luanlouis/article/details/39892027)
    + [1.2 class文件中的常量池](http://blog.csdn.net/luanlouis/article/details/40148053)
      + [1.2.2 Class文件中的常量池详解（上）](http://blog.csdn.net/luanlouis/article/details/39960815)
      + [1.2.3 Class文件中的常量池详解（下）](http://blog.csdn.net/luanlouis/article/details/40301985)
    + [1.3 class文件中的访问标志、类索引、父类索引、接口索引集合](http://blog.csdn.net/luanlouis/article/details/41039269)
    + [1.4 class文件中的字段表集合--field字段在class文件中是怎样组织的](http://blog.csdn.net/luanlouis/article/details/41046443)
    + [1.5 class文件中的方法表集合--method方法在class文件中是怎样组织的](http://blog.csdn.net/luanlouis/article/details/41113695)
  + [2. 格式修正用](####)(用来使排版美观一点:-))
  + [3. JVM运行时数据区](http://blog.csdn.net/luanlouis/article/details/40043991)
  + [4. JVM机器指令集](http://blog.csdn.net/luanlouis/article/details/50412126)
  + [5. JVM类加载器机制与类加载过程](http://blog.csdn.net/luanlouis/article/details/50529868)

### 10.3 Java虚拟机

> 作者：[五月的仓颉](https://www.cnblogs.com/xrq730/category/731395.html)
>

+ [Java虚拟机1：什么是Java](https://www.cnblogs.com/xrq730/p/4826691.html)
+ [Java虚拟机2：Java内存区域及对象](https://www.cnblogs.com/xrq730/p/4827590.html)
+ [Java虚拟机3：常用JVM命令参数](https://www.cnblogs.com/xrq730/p/4830692.html)
+ [Java虚拟机4：内存溢出](https://www.cnblogs.com/xrq730/p/4833713.html)
+ [Java虚拟机5：Java垃圾回收（GC）机制详解](https://www.cnblogs.com/xrq730/p/4836700.html)
+ [Java虚拟机6：内存溢出和内存泄露、并行和并发、Minor GC和Full GC、Client模式和Server模式的区别](https://www.cnblogs.com/xrq730/p/4839245.html)
+ [Java虚拟机7：内存分配原则](https://www.cnblogs.com/xrq730/p/4841177.html)
+ [Java虚拟机8：虚拟机性能监控与故障处理工具](https://www.cnblogs.com/xrq730/p/4842483.html)
+ [Java虚拟机9：Java类加载机制](https://www.cnblogs.com/xrq730/p/4844915.html)
+ [Java虚拟机10：类加载器](https://www.cnblogs.com/xrq730/p/4845144.html)
+ [Java虚拟机11：运行期优化](https://www.cnblogs.com/xrq730/p/4857820.html)
+ [Java虚拟机12：Java内存模型](https://www.cnblogs.com/xrq730/p/4859107.html)
+ [Java虚拟机13：互斥同步、锁优化及synchronized和volatile](https://www.cnblogs.com/xrq730/p/4978876.html)
+ [Java虚拟机14：Java对象大小、对象内存布局及锁状态变化](https://www.cnblogs.com/xrq730/p/6928133.html)
+ [Java虚拟机15：再谈四种引用状态](https://www.cnblogs.com/xrq730/p/7082471.html)
+ [Java虚拟机16：Metaspace](https://www.cnblogs.com/xrq730/p/8688203.html)

### 10.4 RednaxelaFX的博客

> 作者：[RednaxelaFX](http://rednaxelafx.iteye.com/)
>

R大曾经在Oracle虚拟机组工作过，对虚拟机的理解无论是理论还是代码十分厉害，他个人的博客下有许多文章，读者可根据需要自由选择，不过貌似已经不更新了。

+ [自己关于VM的帖的目录](http://rednaxelafx.iteye.com/blog/362738)

### 10.5 你假笨的博客

> 作者：[你假笨](http://lovestblog.cn/)
>

+ [文章](http://lovestblog.cn/)

### 10.6 JVM实用参数系列

> 原作者：[Sven Ruppert](https://blog.codecentric.de/en/)

> 译者：[并发编程网](http://ifeve.com)

+ [JVM实用参数系列](http://ifeve.com/useful-jvm-flags/)
  + [JVM实用参数（一）JVM类型以及编译器模式](http://ifeve.com/useful-jvm-flags-part-1-jvm-types-and-compiler-modes-2/)
  + [JVM实用参数（二）参数分类和即时（JIT）编译器诊断](http://ifeve.com/useful-jvm-flags-part-2-flag/)
  + [JVM实用参数（三）打印所有XX参数及值](http://ifeve.com/useful-jvm-flags-part-3-printing-all-xx-flags-and-their-values/)
  + [JVM实用参数（四）内存调优](http://ifeve.com/useful-jvm-flags-part-4-heap-tuning/)
  + [JVM实用参数（五）新生代垃圾回收](http://ifeve.com/useful-jvm-flags-part-5-young-generation-garbage-collection/)
  + [JVM实用参数（六）吞吐量收集器](http://ifeve.com/useful-jvm-flags-part-6-throughput-collector/)
  + [JVM实用参数（七）CMS收集器](http://ifeve.com/useful-jvm-flags-part-7-cms-collector/)
  + [JVM实用参数（八）GC日志](http://ifeve.com/useful-jvm-flags-part-8-gc-logging/)

## 11 编程练习

### 11.1 使用Go语言编写的虚拟机

> 作者：[zxh0](https://github.com/zxh0)
>
> 语言：go

jvm.go的编写者是《自己动手写Java虚拟机》的作者，参照书籍应该能方便读者理解。

+ github：[jvm.go](https://github.com/zxh0/jvm.go)

### 11.2 使用C++编写的虚拟机

> 作者：[Cthulhu](http://blog.csdn.net/racaljk)
>
> 语言：C++

+ github：[yvm](https://github.com/racaljk/yvm)
+ wiki：[wiki](https://github.com/racaljk/yvm/wiki)

### 11.3 使用Java编写的虚拟机

#### 11.3.1 使用Java编写的虚拟机

> 作者：[kevinlynx](http://codemacro.com)
>
> 语言：Java

该项目由相关配套的文章，一起食用效果更好

+ github：
  + [toy_jvm](https://github.com/kevinlynx/toy_jvm)
  + [toy_jit](https://github.com/kevinlynx/toy_jit)

+ 文章：
  + [写一个玩具Java虚拟机](http://codemacro.com/2017/02/25/toy-jvm/)
  + [实现JVM中的JIT](http://codemacro.com/2017/03/09/toy-jit/)

#### 11.3.2 使用Java编写的虚拟机

> 作者：[caoym](https://www.jianshu.com/u/0f957286095b)
>
> 语言：Java

该项目也有相关配套的文章，实现了一个刚好能够运行HelloWorld的简单虚拟机

+ github：[jjvm](https://github.com/caoym/jjvm)

+ 文章：
  + [用Java实现JVM（一）：刚好够运行 HelloWorld](https://www.jianshu.com/p/4d81465c2fb8)
  + [用Java实现JVM（二）：支持接口、类和对象](https://www.jianshu.com/p/d057e4aa5fcc)

#### 11.3.3 使用Java编写的虚拟机

> 作者：[zachaxy](https://zachaxy.github.io/)
>
> 语言：Java

+ github：[JVM](https://github.com/zachaxy/JVM)

## 12 书籍

### 12.1 深入理解Java虚拟机

国内目前来说最好的JVM相关书籍，周先生的水平毋庸置疑。在此书发行之前，国内好像没有一本完整介绍JVM的书籍。另外，目前市面上也有几本与JVM相关的书籍，评价多半是不好的，有的是抄袭，有的是内容比较浅，有的是作者本身就没有搞清楚就大写特写，另外有的全篇充斥大段代码，充占篇幅。

> 作者：周志明
>
+ 《深入理解Java虚拟机:JVM高级特性与最佳实践》

### 12.2 垃圾回收的算法与实现

介绍了垃圾回收的算法，该书分为两个部分，算法篇和实现篇。算法篇描述时使用伪代码来描述，脱离了具体的语言，实现篇需要有一定的C/C++的基础
才能较好地理解，另外本书的翻译稍显生硬，如果有能力建议读者直接阅读日文原版为好。

> 作者：中村成洋
>
+ 《垃圾回收的算法与实现》

### 12.3 自己动手写Java虚拟机

作者从0开始一步一步教读者写一个较为完整的虚拟机，虽然说该虚拟机是使用go语言编写的，但是如果读者使用过其他编程语言，也应该没有问题。

> 作者：张秀宏
>
+ 《自己动手写Java虚拟机》


## 13 最后

如果有好的文章，书籍，欢迎提pull request。一起交流，一起进步。


## 更新日志

+ 重新整理格式(2019-01-22)
+ 目录整理，内容小范围修改(2019-01-23)
+ 添加[五月的仓颉]系列文章(2019-01-28)
+ 添加新的内容，JVM有关的问题(2019-02-01)
+ 添加[并发编程网]系列文章(2019-03-12)
+ 添加[你假笨]文章(2019-04-05)
+ 添加[先有蛋还是先有鸡]问题(2019-04-09)
+ 添加[JVM简史]文章(2019-04-15)
+ 添加[添加lambda表达式]相关文章(2019-04-23)
+ 添加[InvokeDynamic]文章(2019-04-28)
+ 添加[Java值传递]文章(2019-10-24)
