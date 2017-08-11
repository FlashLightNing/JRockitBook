# 11 JRCMD {#11-jrcmd}

本章将会对JRockit发行版中最简单的工具JRCMD做详细介绍。JRCMD是个命令行工具，可以列出系统上正在运行的所有JRockit JVM，并于其中的某个实例进行交互，执行相关操作。

本章主要内容如下：

* 如何使用JRCMD列出系统上所有正在运行的JVM实例；
* 如何使用JRCMD在运行中的JVM执行诊断指令；
* 如何覆盖JRockit JVM中对
  `SIGQUIT`
  信号的默认处理操作；
* 如何使用JRCMD完成如下任务：
 
  * 堆分析
  * 异常分析
  * 追踪本地内存
  * 控制Management Server的生命周期
  * 通过命令行控制JFR

在本章的最后，是JRCMD的参考文档，按字母表顺序列出JRCMD中的诊断指令，并辅以相应的示例。

