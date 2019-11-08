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

## macOS 是什么

![1991-2009](https://vignette.wikia.nocookie.net/logopedia/images/b/b9/MacOS_original_logo.svg/revision/latest/scale-to-width-down/55?cb=20180926062635)
![2012](https://vignette.wikia.nocookie.net/logopedia/images/0/08/The_OS_X_Logo.svg/revision/latest/scale-to-width-down/80?cb=20180926062134)
![macOS](https://vignette.wikia.nocookie.net/logopedia/images/2/21/MacOS_wordmark_%282017%29.svg/revision/latest/scale-to-width-down/80?cb=20180926061551)

**macOS**（/ˌmækʔoʊˈɛs/；2011年及之前称 **Mac OS X**，2012年至2015年称 **OS X**）是苹果公司推出的基于图形用户界面操作系统，为**麦金塔 (Macintosh)** 的主操作系统。

macOS 架构图
![img](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f2/Diagram_of_Mac_OS_X_architecture.svg/556px-Diagram_of_Mac_OS_X_architecture.svg.png)

***

# 再回头看一下操作系统的结构
**操作系统基本框架**
![img](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d8/Operating_system_architecture.svg/400px-Operating_system_architecture.svg.png)
**Windows**
![img](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5d/Windows_2000_architecture.svg/468px-Windows_2000_architecture.svg.png)
**Linux**
![img](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3a/Linux_kernel_ubiquity.svg/800px-Linux_kernel_ubiquity.svg.png)
**macOS**
![img](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f2/Diagram_of_Mac_OS_X_architecture.svg/556px-Diagram_of_Mac_OS_X_architecture.svg.png)
**Harmony OS 鸿蒙**
![img](https://pic2.zhimg.com/80/v2-49e19902943af0ad916da1bef01ec9fb_hd.jpg)

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

## 内核的分类
内核在设计上可以概分为宏内核与微内核两大架构。

* 宏内核   
如 ```Unix```、```BSD```、```DOS```、```Unix-Like```、```Linux```等

* 微内核  
如 ```Minix```、```QNX```、```Hurd```等

* 混合内核  
如 ```Windows NT```、```Mach```、```XNU```等

***

### 宏内核
**宏内核**定义出一个高端的虚拟接口，由该接口来涵盖描述整个电脑硬件，这些描述会集合成一组硬件描述用词，有时还会附加一些系统调用 (System Call)，如此可以用一个或多个模块来实现各种操作系统服务，如进程管理、并发（Concurrency）控制、存储器管理等。

**宏内核**被视作为运行在单一地址空间的单一的进程，内核提供的所有服务，都以特权模式，在这个大型的内核地址空间中运作，这个地址空间被称为**内核态（kernel space）**。  
它通常是以单一静态二进制文件的方式被存储在磁盘，或是缓冲存储器上，在引导之后被加载存储器中的内核态，开始运作。  

**用人话来说就是：宏内核接管了所有的计算机资源。**  
即：中央集权。

**优点：**
> 设计简单，因为**高度紧密性**所以性能优良。  
> 性能优良：内核之中的通信成本很小，内核可以直接调用内核态内的函数，跟用户态的应用程序调用函数一样，因此它的性能很好。

**缺点：**
> 移植性不佳，因为**高度紧密性**所以可靠性不如微内核。
> 可靠性：所有的模块也都在同一块定址空间内运行，倘若某个模块有错误、瑕疵（Bug），运行时就会损及整个操作系统运作。

***

### 微内核
**微内核**由一群尽可能将数量最小化的软件程序组成，它们负责提供、实现一个操作系统所需要的各种机制与功能。这些最基础的机制，包括了底层地址空间管理，线程管理，与行程间通信（IPC）。

**用人话来说就是：这是一堆内核。**

**微核心**的设计理念，是将系统服务的实现，与系统的基本操作规则区分开来。它实现的方式，是将核心功能模块化，划分成几个独立的行程，各自运行，这些行程被称为服务（service）。所有的服务行程，都运行在不同的地址空间。只有需要绝对特权的行程，才能在具特权的运行模式下运行，其余的行程则在用户空间运行。

**优点：**
> 易于实现与调试，增进可移植性，系统稳定度增加，功能更有弹性。
> 微内核避免了单一组件失效导致整个系统崩溃，内核只需要重启这个组件即可。微内核甚至可以抽换或新增某些服务行程，使功能更有弹性。

**用人话来说就是：零件坏了就换，想要功能就加装：**  
> M4 MWS模组化武器系统:
![M4MWS](https://upload.wikimedia.org/wikipedia/commons/thumb/1/19/M4w-att.jpg/500px-M4w-att.jpg)

**缺点：**
> 性能不佳，性能不佳，性能不佳。
> 行程间通信耗费的资源与时间，比简单的函数调用还多；通常又会涉及到核心空间到用户空间的环境切换（context switch）。这使得消息传递有延迟，以及传输量（throughput）受限的问题，因此微核心在通信宽容度不足下，可能出现性能不佳的问题。

**用人话来说就是：根据中学历史知识，中央集权制度最具有效率。**
即：宏内核性能肯定是最好的啦。

***

### 混合内核
**混合核心**的基本设计理念，是以微核心架构来设计操作系统核心，但在实现上则采用宏内核的作法。混合核心实质上是微核心，只不过它让一些微核结构运行在用户空间的代码运行在核心空间，这样让核心的运行效率更高些。这是一种妥协做法，设计者参考了微核心结构的系统运行速度不佳的理论。

林纳斯·托瓦兹认为，采用可加载核心模块不代表这个操作系统就是一种混合核心，如果模块跟内核使用同样的定址空间，能够访问内核的数据结果，这种实现方式就是宏内核。以这种定义来看，混合核心实际上是宏内核的变种。

**用人话来说就是：根据中学历史知识，皇帝有了宰相。**

**优点：**
> 宏内核的优点，微内核的优点。

**缺点：**
> 没有宏内核的缺点，没有微内核的缺点。

***