# 6 JRockit Mission Control套件 {#6-jrockit-mission-control套件}

作为Java运行时，人们期望JRockit能够持续稳定地监控Java应用程序的运行情况。正如在之前几章介绍的，在Java应用程序运行过程中，JRockit有很多事情要做，例如找出哪些方法最耗时间，以及跟踪内存使用情况和应用程序的内存分配行为（因为如果发生内存泄漏的情况就不太妙了）。

在对应用程序做性能分析或诊断时，JRockit所收集到的运行时数据将会是非常宝贵的资料。

在本书的第2部分中，将会对JRockit所提供的套件工具做详细介绍。在接下来的4章中，将对JRockit发行版中工具做介绍，分别是JRockit Mission Control，JRockit Runtime Analyzer（在R28版本中，该工具已被JRockit Flight Recorder取代），JRockit Memory Leak Detector和JRCMD。

上述的前3个工具均包含在JRockit Mission Control套件中，最后一个，即JRCMD，是一个命令行工具，随JRockit JDK一起发布。这些工具都可以连接到正在运行的JVM上，再完成各自的工作，此外，它们的执行开销都非常小，可以应用于生产环境。

本章的主要知识点包括：

* JRockit Mission Control的两种启动方式，独立启动和作为Eclipse Ide的插件启动
* 配置JRockit JVM以便可以通过JRockit Mission Control进行远程管理
* 配置JRockit Mission Control以便可以使其自动发现其他正在运行的JRockit JVM
* 配置JRockit JVM中的管理代理（Management Agent）
* 安全使用JRockit Mission Control和JRockit Management Agent
* 处理JRockit Mission Control和JRockit JVM的连接问题
* 从JRockit Mission Control中获取更多调试信息
* 介绍JRockit Mission Control的Experimental Update Site，以及如何扩展JRockit Mission Control

本章的部分内容涉及到Eclipse IDE，希望读者能预先了解一下相关内容，更多与Eclipse IDE相关的内容请参见[http://www.eclipse.org](http://www.eclipse.org)。

