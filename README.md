# 微机原理 && 汇编语言
> 摘要：<br>硬件基础：1、微型计算机CPU的内部构造，指令执行逻辑；2、定时器构造及工作原理。<br>汇编语言：1、寻址方式；2、常用指令。
> 前言：<br>理解微型计算机的底层结构和工作原理，有助于更好地学习和体会高级编程语言的工作机制；如作用域、原型对象、继承的理解，结合计算机的内存机制可以更加清晰的体会其本质原理。

### 一、CPU内部结构
#### 1、知识框架
![image](https://github.com/Liquan-gdut/-80x86-Micro-computer-theory/blob/master/CPU.png)

#### 2、寻址、运算大致流图
![image](https://github.com/Liquan-gdut/-80x86-Micro-computer-theory/blob/master/%E4%BB%A3%E7%A0%81%E8%BF%90%E8%A1%8C%E5%A4%A7%E8%87%B4%E6%B5%81%E5%9B%BE.png)
#### 小结：<br>
CPU的本质作用：①存放“代码/数据”，找到“代码/数据”的位置（寻址）；②进行相应的“运算”，送回运送结果。<br>
重点理解：①程序在底层“流动执行”的过程；②高级语言中的“原型链、继承、作用域、垃圾回收、内存泄漏”等知识的理解应结合其物理内存结构。<br>

### 二、汇编语言

#### 1、寻址方式

(1)立即寻址<br>
   机制：将数据存放在“存储器的静态存储区”当中，与程序代码同一片区域，访问速度最快。<br>
(2)寄存器寻址<br>
   机制：将数据存放在“通用寄存器”当中，访问速度仅次于“立即寻址”。<br>
(3)存储器寻址<br>
   机制：将数据存放在“存储器”当中，访问速度较慢（实际也很快），当寻址范围较大。<br>

#### 2、常用指令
![image](https://github.com/Liquan-gdut/-80x86-Micro-computer-theory/blob/master/masm.png)

#### 小结：<br>
汇编与高级的区别：汇编需要明确知道数据在哪个位置，才能进行下一步运算；高级只需通过变量/对象名进行运算即可。
