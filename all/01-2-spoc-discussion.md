# lec1: 操作系统概述

---

## **提前准备**

（请在上课前完成）

* 完成lec1的视频学习和提交对应的在线练习
* git pull ucore\_os\_lab, ucore\_os\_docs, os\_tutorial\_lab, os\_course\_exercises in github repos。这样可以在本机上完成课堂练习。
* 知道OS课程的入口网址，会使用在线视频平台，在线练习/实验平台，在线提问平台\(piazza\)
  * [http://os.cs.tsinghua.edu.cn/oscourse/OS2019spring](http://os.cs.tsinghua.edu.cn/oscourse/OS2019spring)


* 会使用linux shell命令，如ls, rm, mkdir, cat, less, more, gcc等，也会使用linux系统的基本操作。
* 在piazza上就学习中不理解问题进行提问。



# 思考题

## 填空题

* 当前常见的操作系统主要用C, C++, ASM编程语言编写。
* "Operating system"这个单词起源于Operator 。
* 在计算机系统中，控制和管理各种资源、有效地组织多道程序运行的系统软件称作操作系统 。
* 允许多用户将若干个作业提交给计算机系统集中处理的操作系统称为批处理操作系统
* 你了解的当前世界上使用最多的操作系统是Android 。
* 应用程序通过系统调用接口获得操作系统的服务。
* 现代操作系统的特征包括并发性 ， 虚拟性 ， 异步性 ，持久性 。
* 操作系统内核的架构包括宏内核 ， 微内核 ， 外核 。


## 问答题

- 请总结你认为操作系统应该具有的特征有什么？并对其特征进行简要阐述。
  - 操作系统具有的特征有虚拟性，并发性，异步性，共享性和持久性
  - 虚拟性：虚拟化技术常用于操作系统中，它将各种实体资源转化成逻辑上的虚拟资源供应用使用，例如虚拟内存、虚拟处理器、虚拟外部设备。
  - 并发性：宏观上操作系统具有处理多道程序同时执行的能力，并且能够同时应对各种异常和错误。
  - 异步性：多道程序环境下，允许多个程序并发执行，但单个进程的执行是时走时停的。
  - 共享性：操作系统提供的资源可以供内存中多个并发执行的进程共同使用。
  - 持久性：操作系统可以将程序和数据等永久保存在磁盘中。


- 为什么现在的操作系统基本上用C语言来实现？为什么没有人用python，java来实现操作系统？

  - 因为C语言具有高效的性能，能嵌入汇编，直接操作硬件，python和java性能相比较低，不能直接操作硬件。

---

## 可选练习题

---

- 请分析并理解[v9\-computer](https://github.com/chyyuu/os_tutorial_lab/blob/master/v9_computer/docs/v9_computer.md)以及模拟v9\-computer的em.c。理解：在v9\-computer中如何实现时钟中断的；v9 computer的CPU指令，关键变量描述有误或不全的情况；在v9\-computer中的跳转相关操作是如何实现的；在v9\-computer中如何设计相应指令，可有效实现函数调用与返回；OS程序被加载到内存的哪个位置,其堆栈是如何设置的；在v9\-computer中如何完成一次内存地址的读写的；在v9\-computer中如何实现分页机制。


- 请编写一个小程序，在v9-cpu下，能够输出字符


- 输入的字符并输出你输入的字符


- 请编写一个小程序，在v9-cpu下，能够产生各种异常/中断


- 请编写一个小程序，在v9-cpu下，能够统计并显示内存大小



- 请分析并理解[RISC-V CPU](http://www.riscvbook.com/chinese/)以及会使用模拟RISC\-V(简称RV)的qemu工具。理解：RV的特权指令，CSR寄存器和在RV中如何实现时钟中断和IO操作；OS程序如何被加载运行的；在RV中如何实现分页机制。
  - 请编写一个小程序，在RV下，能够输出字符
  - 输入的字符并输出你输入的字符
  - 请编写一个小程序，在RV下，能够产生各种异常/中断
  - 请编写一个小程序，在RV下，能够统计并显示内存大小

## 参考资料
 - [Intel格式和AT&T格式汇编区别](http://www.cnblogs.com/hdk1993/p/4820353.html)
 - [x86汇编指令集  ](http://hiyyp1234.blog.163.com/blog/static/67786373200981811422948/)
 - [PC Assembly Language, Paul A. Carter, November 2003.](https://pdos.csail.mit.edu/6.828/2016/readings/pcasm-book.pdf)
 - [*Intel 80386 Programmer's Reference Manual*, 1987](https://pdos.csail.mit.edu/6.828/2016/readings/i386/toc.htm)
 - [IA-32 Intel Architecture Software Developer's Manuals](http://www.intel.com/content/www/us/en/processors/architectures-software-developer-manuals.html)
 - [v9 cpu architecture](https://github.com/chyyuu/os_tutorial_lab/blob/master/v9_computer/docs/v9_computer.md)
 - [RISC-V cpu architecture](http://www.riscvbook.com/chinese/)
 - [OS相关经典论文](https://github.com/chyyuu/aos_course_info/blob/master/readinglist.md)
