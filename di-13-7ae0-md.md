# 13 JRockit Virtual Edition {#13-jrockit-virtual-edition}

近些年，**虚拟化（virtualization，即在模拟硬件上运行软件）**，可谓是风头正劲。通过虚拟化可以最大化硬件资源利用率，同时可以简化资源管理。不过，作为应用程序和实际硬件中间的抽象层，虚拟化会带来额外的性能损耗。

本章将会对JRockit Virtual Edtion及其相关技术进行介绍。在本章中，会以JRockit VE作为JRockit Vritual Edtion的简称使用。

JRockit VE使用户可以在一个没有操作系统的虚拟环境中运行Java应用程序，同时免去了虚拟化所带来的大量性能损耗。JRockit VE是一款独立的产品，包含了运行Java应用程序所需要的最小环境，即一个轻量级的类OS内核和一个JRockit JRE。

JRockit VE可以运行任何Java应用程序，不过最初可能更多的是作为**WLS on JRockit VE（WebLogic Server on JRockit Virtual Edtion）**产品的一部分来使用。WLS on JRockit VE是以虚拟机镜像（virtual machine image）格式预先打包好的WebLogic Server安装文件。虚拟机镜像是一个二进制镜像，其中包含了虚拟机配置，二进制软件和文件系统，将虚拟机镜像部署在专门的虚拟环境（例如Oracle VM Server）中，就可以运行相应的应用程序。

作为对JRockit VE相关技术的介绍，本章会着重讲解虚拟化JRockit VE背后的相关技术。对于构建与JRockit VE之上的软件栈，则不再赘述。

> 本章旨在介绍新近技术产品，因此在细节、名称和具体实现上可能会因与目前所见到的有所区别，而且在本章中还有一些前瞻性的、还未实现的技术介绍。万变不离其宗，不论如何，核心概念上是相同的。相关产品的最新信息可以在官网的在线文档上查看。

本章主要包含以下内容：

* 虚拟化的基本概念以及几种不同的虚拟化实现的相关介绍
* Hypervisor相关介绍
* 软件栈虚拟化的优劣
* Java虚拟化的相关问题，以及JRockit VE简化虚拟化进程并提升性能的方法
* 虚拟机镜像相关概念
* 虚拟化的未来



