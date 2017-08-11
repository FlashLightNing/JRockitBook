# 12 JRockit Management API {#12-jrockit-management-api}

JRockit的管理功能非常有用，访问方式也有很多，但它们并未写入到正式的文档中，因此在不同的JRockit版本之间可能有所不同。应用程序若依赖于这些API，则可能无法部署在所有的JRockit版本中。尽管如此，本章还是会对这些API做相应的介绍，因为它们确实非常有用。

本章主要包含以下内容：

* 如何通过
  **JRockit Management API（JMAPI）**
  访问JRockit JVM中的运行时信息；
* 如何初始化不同版本JRockit中的JMX-based JRockit Management API（JMXMAPI）

> 在JRockit R28版本中，JMAPI已经被部分废弃了，而JRockit的所有版本都已经不再支持JMXMAPI。



