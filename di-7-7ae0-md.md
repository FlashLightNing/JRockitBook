# 7 Management Console {#7-management-console}

最先集成到JRockit Mission Control套件中的工具是JRockit Management Console，它可以用来监控JRockit JVM，以及运行在其中的应用程序，此外还可以修改JRockit JVM中某些运行时状态。阅读本章时，请先对[JMX相关技术](http://www.oracle.com/technetwork/java/javase/tech/javamanagement-140525.html)做简要了解。

> 更多有关JMX的内容参见[http://java.sun.com/javase/technologies/core/mntr-mgmt/javamanagement/](http://java.sun.com/javase/technologies/core/mntr-mgmt/javamanagement/)

Management Console基于JMX实现，应用程序和JRockit JVM通过JMX主动暴露出管理接口。

本章的主要内容如下：

* 如何启动Management Console
* 如何监控MBean的属性
* 如何调用MBean的操作
* 如何创建触发规则
* 如何启用死锁检查
* 如何执行基于线程的内存分配和CPU分析
* 诊断命令简介
* 如何扩展Management Console



