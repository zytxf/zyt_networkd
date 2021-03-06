# 为什么要学好c语言，c语言到底多重要

 	

## 一、前言

对于理工 科学生来说，这个答案可能很简单，因为这是一门必修课。而对于程序员来说选择一门编程语言，在某种程度上，对职业生涯的发展会产生重大的影响，所以必须慎 之又慎。那么，为什么要选择一门诞生了将近半个世纪的语言？本文不是老生常谈的废话，如：”C 语言是编程的基础”、”学好 C 语言，走遍天下都不怕”等等，本文力争详尽而又有理的回答这个问题，旨在成为最好的为什么要学习和使用 C 的文章。

## 二、C 语言

C 语言是由美国 AT&T 贝尔实验室的研究员 Dennis Ritchie 在 B 语言的基础上，最初作为改造 Unix 操作系统的开发语言，并伴随着 Unix 操作系统兴起而流行，后来，随着微型计算机的发展，C 开始被移植到其他操作系统平台上，成为独立的程序设计语言。

**下图摘自 TIOBE 编程语言排行榜，过去 30 年 90% 时间里 C 都是独领风骚的，仅偶尔被 Java 超越：**

![为什么要学习和使用 C 语言？](http://www.itjs.cn/uploads/allimg/151211/122P53609-0.png)

**技术分享**

那么是因为一门语言一直位于排行榜的第一名就该去学习和使用吗？显然不是，人云亦云是程序员的大忌。为操作系统而生的标签注定了 C 不可能平庸，实话实说，C 是一门很难学习和使用的编程语言，没有编译原理、操作系统和计算机体系结构扎实的基础知识，根本不可能把 C 学的明白、用的顺手。C 作为一门工程实用性极强的语言，提供了对操作系统和内存的精准控制，高性能的运行时环境，源码级的跨平台编译等优点，才是我们必须学习和使用 C 的理由。

同时，幸运的是 C 也是个有趣的东西，对编程的认知越深，就会越觉得有意思，我简单列举一些 C 的优点：

2.1）结构化设计语言，语法清晰、结构简单，模块化使得程序的各个部分除了必要的信息交流外彼此独立，便于开发、调试以及调试。

2.2）运算符多，把括号、赋值、强制类型转换等都作为运算符处理，灵活使用各种运算符可以实现在其它高级语言中难以实现的运算。

2.3）数据结构丰富，能实现各种复杂的数据类型的运算，引入指针、结构体概念使程序效率更高。

2.4）为操作系统而生，可以像汇编语言一样对位、字节和地址进行操作，允许直接访问物理地址对硬件进行操作，把高级语言的基本结构和语句与低级语言的实用性结合起来。

2.5）程序执行效率高，一般比汇编程序生成的目标代码效率低 10%~20%。

2.6）可移植性好，C 语言抽象了针对 CPU 编程的细节，能广泛应用于针对大型操作系统和系统软件的编写。

2.7）具备强大的绘图功能，和 C++ 一样也可以写出很优雅的二维、三维图形和动画。

有人说，C 是 C++ 的子集，C 能做到的事，C++ 一样能做到，并且还可以做的更好，如：三大面向对象特性、GUI 编程，诚然，我承认在 GUI 编程领域 C++ 占据着绝对的统治地位，至今无人能撼动。但真的有必要用 C++ 来替代 C 完成工作吗？很多时候 C++ 解决问题的思路真的比 C 更先进吗？

## 三、C 和 C++ 比较

写到这一 段的时候我有一种战战兢兢、如履薄冰的感觉，毕竟 C、C++ 是广大程序员都很熟悉东西，打起嘴炮来也是极其恐怖的，其实在关乎信仰的问题上，任何的争论都是无止境的，也是无意义的。我希望大家不要把大量精力用来争 论纯粹的语言优劣上，而是去思考如何的正确的把事情做好，什么是正确的做事——快速高效的开发，保障快速稳定的运行，快速简单的维护。

下图是嘴炮大神 Linus Torvalds 当年抨击 C++ 和他周围那些 C++ 大牛程序员们的犀利言辞，其实我个人并不欣赏 Linus 的个人风格，我还是希望大家能心平气和的谈谈 C 相比 C++ 的一些优点和现状：

![为什么要学习和使用 C 语言？](http://www.itjs.cn/uploads/allimg/151211/122P512R-1.png)

**技术分享**

3.1）隐式操作：C 简单直接、结构清晰，每行代码都能清楚的被反汇编成相应的语句，系统会严格按照你的代码去执行。而 C++ 则不尽然，简单的语句也说不清楚究竟有多少次构造和拷贝，这样编写底层代码是完全不行的，底层需要精准和严格的控制。

3.2） 语言接口：现代软件工程项目的开发，不但对性能有很高要求，对于语言接口的对接能力也有很高要求，因为偌大的一个项目很少仅使用一种语言来进行开发，对于 底层，C++ 对内存和硬件的控制不如 C 简洁精准；对于很多动态语言和中间件，如：PHP、Python 和 Apache、Redis，都受了 C 的很大影响，甚至就是 C 开发出来的东西，对接起来非常方便。没错儿，其实 C++ 采用迂回的方式也能对接的，但是，远远不如 C 方便，开发和维护成本非常高。

3.3）硬件层：

3.2.1>分配内存：系统加电后运行，经过汇编初始化栈，然后再跳转到 C 语言的 start_init() 函数去，这时候内存分配机制都还没有建立，C++ 如何定义类？如何实例化对象？

3.2.2>标准库依赖：C 的所有特性都可以不依赖任何库运行，如有必要，可以按照特定需求自己编写库。

3.2.3>处理器兼容：C++ 的类是依赖基地址+偏移地址的寻址方式，很多微处理器只有简单的给定地址寻址，不支持一条语句实现 base + offset 的寻址机制，很多 C++ 代码编译出来需要更多的指令来运算地址，导致性能下降了太多。

3.4）应用层：C++ 在做应用层尤其是 GUI 编程，这是 C++ 的传统强项，我一直坚持 C 也能优雅的做出图像和动画，但开发效率确实较 C++ 低很多，最近有个很火的 RUST 语言，号称是未来唯一能取代 C++ 的编程语言，感兴趣的同学可以多关注下。

## 四、总结

![为什么要学习和使用 C 语言？](http://www.itjs.cn/uploads/allimg/151211/122P545J-2.png)

下面我列举了 10 多个目前热门的发展方向，粗略的介绍了下列项目里最常用的编程语言：技术分享

由上图可知，操作系统、编译原理、数据结构与算法等等基础知识，是深入理解、掌握和灵活运用 C 的重要前提，现阶段程序员职业生涯超过一半的热门方向直接或间接与 C 有关，我想，学好 C 的重要性也就不言而喻了。