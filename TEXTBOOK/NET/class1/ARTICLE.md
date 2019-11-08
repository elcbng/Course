# 操作系统与 Linux 介绍

## 操作系统是什么

> **操作系统**（英语：**O**perating **S**ystem，缩写：**OS**）是管理计算机硬件与软件资源的**系统软件**，同时也是计算机系统的内核与基石。操作系统需要处理如管理与配置内存、决定系统资源供需的优先次序、控制输入与输出设备、操作网络与管理文件系统等基本事务。操作系统也提供一个让用户与系统交互的操作界面。

**操作系统**，简单来说就是为了**简化**用户操作计算机而存在的。

***

### 操作系统的分类

**操作系统的分类并没有一个单一的标准。**

根据工作方式分类：批处理操作系统、分时操作系统、实时操作系统、网络操作系统、分布式操作系统等

根据运行的环境分类：桌面操作系统、嵌入式操作系统等

根据指令长度分类：8bit、16bit、32bit、64bit等

***

### 操作系统的结构

首先，操作系统是个**软件**。

![img](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d8/Operating_system_architecture.svg/400px-Operating_system_architecture.svg.png)

### 操作系统是做什么的

从定义上来讲这个，说实话有点困难。

其实，一个操作系统的成功，取决于多个方面，这也是这节课程的主要话题之一。“**操作系统是什么？**”这个问题过完这节课你就会明白了~~还是不明白~~

***

# 来点例子

***

## Windows 操作系统是什么
![Windows](https://upload.wikimedia.org/wikipedia/commons/thumb/8/8d/Windows_darkblue_2012.svg/800px-Windows_darkblue_2012.svg.png)
**Microsoft Windows**（中译：**视窗操作系统**）是微软公司推出的一系列操作系统。  
~~谁还管这个中译啊~~

**这张图** 是 Windows NT 操作系统家族的体系结构
![img](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5d/Windows_2000_architecture.svg/468px-Windows_2000_architecture.svg.png)

***

## Linux 操作系统是什么

> Linux 的吉祥物 Tux
![Tux](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b0/NewTux.svg/500px-NewTux.svg.png)

**Linux** 是一种自由和开放源码的 **类 UNIX** 操作系统。

**Linux** 严格来说是单指操作系统的内核，因操作系统中包含了许多用户图形接口和其他实用工具。**如今 Linux 常用来指基于 Linux 的完整操作系统，内核则改以Linux内核称之。**

Linux 的作者是 Linus Torvalds
> Linus 的微笑
![Linus](https://upload.wikimedia.org/wikipedia/commons/5/5c/Linus_Torvalds_%28cropped%29.jpg)

**这张图** 是 Linux 的系统架构
![img](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3a/Linux_kernel_ubiquity.svg/800px-Linux_kernel_ubiquity.svg.png)

***

# 再回头看一下操作系统的结构
**操作系统基本框架**
![img](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d8/Operating_system_architecture.svg/400px-Operating_system_architecture.svg.png)
**Windows**
![img](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5d/Windows_2000_architecture.svg/468px-Windows_2000_architecture.svg.png)
**Linux**
![img](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3a/Linux_kernel_ubiquity.svg/800px-Linux_kernel_ubiquity.svg.png)

***

# Kernel 内核

细心的人已经发现，各个操作系统花里胡哨的，但是他们都有一个共同点：

**Kernel**

## 内核是什么

**内核**（英语：**Kernel**）是  
* 用来管理软件发出的数据 I/O（输入与输出）要求的电脑程序  
* 将这些要求转译为数据处理的指令并交由中央处理器（CPU）及电脑中其他电子组件进行处理  
* 是**现代操作系统中最基本的部分**。

> 它是为众多应用程序提供对计算机硬件的安全访问的一部分软件，这种访问是有限的，并由内核决定一个程序在什么时候对某部分硬件操作多长时间。直接对硬件操作是非常复杂的。所以内核通常提供一种硬件抽象的方法，来完成这些操作。有了这个，通过进程间通信机制及系统调用，应用进程可间接控制所需的硬件资源（特别是处理器及IO设备）。

**严格地说，内核并不是计算机系统中必要的组成部分。**  
有些程序可以直接地被调入计算机中执行；这样的设计，说明了设计者不希望提供任何硬件抽象和操作系统的支持；它常见于早期计算机系统的设计中。

但随着电脑技术的发展，最终，一些辅助性程序，例如程序加载器和调试器，被设计到机器内核当中，或者写入在只读记忆体里。这些变化发生时，操作系统内核的概念就渐渐明晰起来了!

***

# Linux 内核 与 Linux 发行版

## Linux 内核 的诞生

### UNIX 的诞生

> 这一切都要从 UNIX 说起。

**UNIX** 是一个强大的多用户、多任务操作系统，支持多种处理器架构，按照操作系统的分类，属于分时操作系统。
最早由 Ken Thompson、Dennis Ritchie 和 Douglas McIlroy 于1969年在AT&T的贝尔实验室开发。

UNIX 曾经开源且允许扩展和修改，并诞生了 **BSD** 等优秀的操作系统。

***

#### 渣男 AT&T

但是随着 AT&T “渐渐露出资本主义的黑暗而又邪恶的欲望”，它对之前的 UNIX 及其变种声明了著作权，并且不再授权 UNIX 的源代码予他人。

AT&T 固执地捍卫 Unix 版权，完全不顾它的创造者和开发者的愿望，导致 Unix 丧失活力、一蹶不振，大量开发者无法参与，只好离开了这个平台。

这引起了很多人的不满，其中包括荷兰阿姆斯特丹自由大学计算机科学系的塔能鲍姆教授（Prof. Andrew S. Tanenbaum）。这个人为了能在课堂上教授学生操作系统运作的实务细节，决定在不使用任何 AT&T 的源代码前提下，自行开发与 UNIX 兼容的操作系统，以避免著作权上的争议。他以小型 UNIX（mini-UNIX）之意，将它称为 **MINIX**。

> **MINIX 与我们有什么关系：**  
所有2015年之后发布的英特尔芯片都在内部运行着 MINIX 3，作为 Intel 管理引擎 (Intel Management Engine) 的组件。

***

#### UNIX / BSD 的衰弱，Windows 与 Linux 的诞生

AT&T 起诉 BSD 侵犯了 Unix 的版权。官司结束以后，BSD不幸发生分裂，变成了 FreeBSD、NetBSD 和 OpenBSD 三个版本。这些原因导致 BSD 直到今天，都还在操作系统的竞争中处在落后地位。

如果换个时间，官司的损失也许还没这么大。偏偏90年代初是计算机工业决定性的年代，错过了那几年，从此你就不要想翻身了。因为从80年代末期开始，Intel的80x86芯片有巨大的发展，性能快速上升，而成本快速下降，个人电脑的年代就要到来了。市场迫切需要能够运行在386芯片上的操作系统，但是Unix和BSD忙于打官司，都没有去做移植操作系统这件事。其他两个这样做的人，改变了人类历史。

**一个是比尔·盖茨，他推出了Windows，占领了个人电脑市场，后来赚了几百亿美元。**

**另一个是芬兰大学生Linus Torvalds，他想学习Unix，但是买不起工作站，就自己写了一个能在386上运行的Linux操作系统，现在全世界超过一半的网络服务器都在使用这个系统。**












## 为什么要用 Linux

以下是 Mike Gancarz 的书《**Linux and the Unix Philosophy**》 序言里面提供了一段具有丰富资讯的一段话：
> Unix 操作系统的开发是起源一个激进的概念：他们假定所有 Unix 操作系统的使用者们，从一开始就是熟悉电脑语言的；所以整套 Unix 哲学都围绕着一件事情“**使用者们知道他自己在做什么**”。

这之中就蕴含了 Linux 精神的真谛：**Linux 从不认为用户能力不足，反而是假定：你明白自己在做什么，并且会遵循你下的任何命令，任何事。无论是有心还是无意。总之，使用者确实掌握了很大的权力。**

### 软件包管理真香
Linux 的软件包管理  
易于安装和卸载  
易于更新已安装的软件包  
保护配置文件  
轻松跟踪已安装文件。

而不是像 Windows 一样下个软件还得去网上找，或者下一个不知道从哪里来的“管家”程序。

### Linux 做开发省心
不说，举个例子：
安装 Java Development Kit：
1. Windows：
> 1. 打开浏览器搜索 JDK 并找到准确的资源下载。
> 1. 找到下载的安装文件并安装。
> 1. 配置环境变量。
> 1. 有时候你可能需要注销来使得环境变量生效。
> 1. 可能完成了。
2. Linux (Ubuntu 为例)
> 1. ```sudo apt-get update && sudo apt-get install openjdk-8-jdk```
> 1. 输入 sudo 密码。
> 1. 好了。

### Linux 强
其实强的不是 Linux，而是给 Linux 和其相关的开源项目做出贡献的程序员们。  
比如说

1. 来自 **戴尔** Linux 团队的 **动态内核模块支持(DKMS)**   
1. 来自 开放虚拟化联盟 的 **基于内核的虚拟机(KVM)**，为**容器**、**云计算**等技术提供了基础。
1. 来自 **谷歌**、**IBM** 等各个大佬的 的 **LXC**
1. 来自 **谷歌** 的 **BBR**，加速网站的访问速度。
1. 来自 **Facebook** 的 **Flashcache** 硬盘缓存加速。
1. 还有难以计数的程序员在为 Linux 做出自己的贡献。

### Linux 协同工作
Linux 可以很多人共同登录进一个服务器里工作。

然而 Windows 只能够同一时间登入有且只有一个用户。

### Linux 清晰
你用 Linux 的时候，你会更容易对操作系统有一个清晰的轮廓。

Windows 与 macOS 等操作系统的哲学，是认为用户本身是不会使用计算机的，它阐述的是：使用者们其实是害怕电脑的，因此必须要让“复杂性”远离使用者。  
**可是，当你选择去“理解”计算机的时候，Windows过于复杂的系统结构简直劝退。**

然而 Linux 结构十分简单，轮廓清晰，上手之后在相对较短时间内就差不多能够理解。

### Linux 完全开源，免费，自由。
GNU/Linux 操作系统从内核到用户程序几乎全程开源。  
你可以阅读整个软件任何部分的源代码。  
你可以修改这些代码。

> GNU代表的自由软件运动相当于争取类似言论自由这样权利的行动，它不同于唯利是图的人，是有信仰的——最终这个道德标准会如同诚信一样普及而人人尊守。

### Total Control
Linux 思想体现在人们可以透过一个终端模拟器，直接连到命令行界面，开始施展使用者的权力。

为了达到更高的灵活度，Linux 甚至有一个荧幕程式，让你可以在单一的终端对话中就能够完成多重对话，这在远端登入时特别有用，因为就算你断线了，荧幕的对话会继续随着所有正在不同外壳里运行的程式工作下去。

> **Linux 的命令行界面 轻声诱惑：它正用它给你的权力在诱惑你。**

**Linux 不会在你下命令的时候踩任何刹车，它假定你很清楚你做的一切是什么，所以你输入什么命令，就会导向什么样的结果，完全不过问，让你完全掌握一切。**

### 尊重每一个使用者。
这就是 Linux 的最高指导原则。

###### rua
塔能鲍姆-托瓦兹辩论
https://blog.csdn.net/chenzhen1080/article/details/82500226