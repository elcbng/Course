# [Java Virtual Machine](https://en.wikipedia.org/wiki/Java_virtual_machine) [(Java虚拟机)](https://zh.wikipedia.org/wiki/Java%E8%99%9A%E6%8B%9F%E6%9C%BA)

Java虚拟机（英语：Java Virtual Machine，缩写为JVM），一种能够运行 Java bytecode 的虚拟机，以堆栈结构机器来进行实做。最早由太阳微系统所研发并实现第一个实现版本，是 Java 平台的一部分，能够运行以 Java 语言写作的软件程序。

Java 虚拟机有自己完善的硬体架构，如处理器、堆栈、寄存器等，还具有相应的指令系统。JVM 屏蔽了与具体操作系统平台相关的信息，使得Java程序只需生成在 Java 虚拟机上运行的目标代码（字节码），就可以在多种平台上不加修改地运行。通过对中央处理器（CPU）所执行的软件实现，实现能执行编译过的 Java 程序码（Applet 与应用程序）。

作为一种编程语言的虚拟机，实际上不只是专用于 Java 语言，只要生成的编译文件匹配JVM对加载编译文件格式要求，任何语言都可以由JVM编译运行。此外，除了甲骨文，也有其他开源或闭源的实现。