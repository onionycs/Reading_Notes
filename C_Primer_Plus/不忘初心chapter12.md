[toc]

# preface

Never forget why you started, and your mission can be accomplished

[不忘初心方得始终](#最想学明白)

# 12 Storage Classes, Linkage, and Memory Management 

The different storage classes offer different combinations of scope, linkage, and storage duration.

> You can have identifiers that can be shared over several files of source code, identifiers that can be used by any function in one particular file, identifiers that can be used only within a particular function, and even identifiers that can be used only within a subsection of a function. 

very big scope to very small one

concurrent programming = 并发编程

exclusively = only

communist party of china (CPC)

communism 共产主义

## Storage Classes 



### Scope Linkage 



### Storage Duration 



### Automatic Variables 



### Register Variables 



### Static Variables with Block Scope 



### Static Variables with External Linkage 

在初始化external variable 时 const int的常量不能用

在数组初始化时const int 的常量不能用，这个const 只是说他不能修改

并不是真正的constant



### Static Variables with Internal Linkage 



### Multiple Files 

读到这里差点把我愉悦送走，满篇的文字看的我头都大了。。

### Storage-Class Specifier Roundup 



### Storage Classes and Functions 



### Which Storage Class? 

need to know principle -> the thought of encapsulation

## A Random-Number Function and a Static Variable 

spontaneity = 自发性

simultaneously = 同时地

操作系统真象还原解释了魔数是什么这里来了一个魔公式

listing 12.9 有点面向对象的语言的感觉了

next封装在类里面，通过srand()成员函数, 改变next这个私有变量

### 最想学明白

1.就是文件流,C语言是怎么把不同操作系统的文件通过统一的流形式进行处理的

进而学会使用printf() scanf() getchar() putchar()

scanf是要的东西前面的whitespace全部扔掉后面的不能翻译的character or whitespace 留下的函数

最后返回成功翻译的items, 是一段翻译程序, 涉及传递参数的压栈过程也只是规规矩矩的32位的地址.

printf是返回输出的字符数(包括\n,punctuation,whitespace),传参过程是依据参数本身的类型进行promote的结果 short char -> int float -> double 因为没有一个包含确切参数类型的prototype对他们进行 typecast ,注意typecast发生的truncation

2.gcc编译C语言source code 的时候怎么在x86和amd64之间转化的在同一台电脑上用怎样的command prompt 命令能过实现用objdump反编译的程序与CSAPP书上反编译的程序一样呢？为什么我这么在乎是64位的还是32位的编译呢，是因为两者的传参模式不一样，64位的操作系统因为多了几个寄存器可以使用，所以前六个参数是用寄存器来传的

3.逆向工程与软件破解

---

感觉用rand() 和srand()函数来阐释静态变量真的是太刁了. 这个地方相当于封装了一个random_number_creator 类.



## Roll ’Em 

dye = die = dice = 骰子  rolling a die you can get 6 outcomes

随机事件是怎么翻译来着, is it *random activity* ? 

>Polyhedral dice
>Everybody knows what a regular 6 sided die is, and, most likely, many of you have already played thousands of games where the one (or more) was used. But, did you know that there are different types of die? Out of the countless possibilities, the most popular dice are included in the Dungeons & Dragons dice set, which contains seven different polyhedral dice:
>
>4 sided dice, also known as a tetrahedron - each face is an equilateral triangle
>6 sided dice, a classic cube - each face is a square
>8 sided dice, also known as an octahedron - each face is an equilateral triangle
>10 sided dice, also known as a pentagonal trapezohedron - each face is a kite
>12 sided dice, also known as a dodecahedron - each face is a regular pentagon
>20 sided dice, also known as an icosahedron - each face is an equilateral triangle
>Don't worry, we take each of these dice into account in our dice probability calculator. You can choose whichever you like, and e.g. pretend to roll five 20 sided dice at once!
>
>cr. <https://www.omnicalculator.com/statistics/dice>

contrived = deliberately created rather than arising naturally or spontaneously.

人为的

emulate = 看齐

match or surpass (a person or achievement), typically by imitation.



coin toss 掷硬币

crap 掷骰子

## Allocated Memory: malloc() and free() 

2021年1月11日15点39分

双精度-double precision

clear this hurdle (an obstacle or difficulty.)



### The Importance of free() 



### The calloc() Function 

allot = allocate

### Dynamic Memory Allocation and Variable-Length Arrays 



### Storage Classes and Dynamic Memory Allocation 

You can think of a program as dividing its available memory into three separate sections: one for static variables with external linkage, internal linkage, and no linkage; one for automatic variables; and one for dynamically allocated memory.

堆、栈、程序正文。

Listing12.15 where.c %p(pointer value)和%zd（size_t）都是%u或者说long为4字节的%lu



## ANSI C Type Qualifiers 

versatile / volatile = changeful

constancy
the quality of being faithful and dependable.
忠诚可靠的品质。

我们需要中文书的原因只是因为一些专业术语terminology的翻译应该统一

而不是因为我们读不懂原版的英语书籍

qualifier 限定符 qualified type 限定类型

qualify = modify = decorate修饰/限制/给予资格

facility noun。facilitate verb。

idempotent  == denoting an element of a set which is unchanged in value when multiplied or otherwise operated on by itself.

幂等 == 表示一组元素，当其自身相乘或以其他方式操作时，其值不变。两个相同的限定符加在一起跟只有一个限定符时效果一样

superfluous = replicated冗余的 赘余的

### The const Type Qualifier 

compliant is a adjective form of comply

precedence of unary operators 单目运算符的优先级

*(p++)； == *p++; 

为什么第二种头文件的使用方式不在每一个都包含一个引用声明呢?之前的头文件就是这样干的

referencing declaration(allow replicated/superfluous) & defining declaration(only once)



### The volatile Type Qualifier 



### The restrict Type Qualifier 

denote indicate = show

imply = hint

you flout it (and) at your own risk 你不遵守它你就危险自负

### The _Atomic Type Qualifier (C11) 



### New Places for Old Keywords 







## Key Concepts 



## Summary 



## Review Questions 



## [Programming Exercises][]

##  



[Programming Exercises]: https://www.weibo.com/ycspro	"weibo"