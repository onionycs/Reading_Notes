# toc

[toc]



# 吐槽

　　1.很讨厌没有首行空两格的中文typesetting.

　　2.首先outline 整个4级标题的全部内容,分工做事,形成用户级的双线程,加大工作效率:smile:

　　3.笔记本电脑用作路由器的可行性，路由器里面最贵的是网卡和天线，笔记本不缺一个好的网卡，只是缺少一个好的天线。

　　4.一个热知识:学了就能经常用的叫热知识,学了偶尔用的叫冷知识,扩大自己的资源获取途径youtube电子书.国外lab帮帮做做,:joy:

　　5.杨mi 的英语名字叫不叫power yang?



# Chapter 3. Data and C

> interest payment or display a sorted list of vintners

利息支付或显示 酒商的排序列表

> merchant(商人) of wine

> as a bonus==reward奖励



## A Sample Program

> wrinkle皱纹

> iron out 熨烫

### Listing 3.1. The `rhodium.c` Program

> pertain = belong

> fiddle with the 14.5833,

`摆弄`noun.`=violin`            verb.`=manipulate`



### What's New in This Program?

> specifier <-- %f 说明符

> displays two places to the right of the decimal.小数点右边显示两位

> notation = symbol

> Together means 合起来



## Data Variables and Constants

> command the obedience = manipulate  a speaker(扬声器)

> cometary orbits 彗星的轨道

> stick=glue=paste=pole(棍子/杆子) figures 简笔画

> bear the information you use 承载着你使用的信息的数据

要修改常量通不过操作系统的优先级审查



## 	Data: Data-Type Keywords

> datum = a piece of information.

> designate = send in charge of = appoint 委派

> $2^8$ can be descripted by 2 times itself 8 times

> 因为我们学的是intel 风格的汇编代码,而intel为了兼容8086的表达,一直把word 定义为16-bits. 但是换成AT&T语法后就会发现不是这回事了,:alien:

### 		Integer Versus Floating-Point Types

> rundown(noun) means an **analysis or summary** of something by a knowledgeable person.



#### 			[The Integer](#toc)

> multiply 3.16 by (10 to the 7th power/by 1 followed by 7 zeros.)
>
> $10^7 * 3.16$



#### 			The Floating-Point Number

> scheme = plan
>
> analogy = similarity 相似的 类比
>
> practical = current
>
> arithmetic operation = 算数的/运算 操作

> subject = control

>7.0 might be stored as a 6.99999 float value—more about precision later.

我们必须有手动帮计算机计算出存在内存中浮点数的能力,我觉得,这样才能深刻的理解`ieee 754`



## 	Basic C Data Types



### 					The `int` Type



#### 								Declaring an `int` Variable

> four `int`-sized variables = 四个`int` 大小的变量





#### 								Initializing a Variable

> assignment operator (=)



#### 								Type `int` Constants

> recognize = appraise / determine / examine



#### 								Printing `int` Values

> The %d is called/termed or of jargon  a *format specifier * 格式说明符

>underlying cause 根本的/底层的 好像是上一章的内容

#### 								[Octal and Hexadecimal](#toc)



#### 								Displaying Octal and Hexadecimal

>If you want to display the C prefixes, you can use specifiers %#o, %#x, and %#X to generate the 0, 0x, and 0X prefixes,

想到了一些人写程序写成

```c
#include<stdio.h>
int main(){
    printf("0x%x\n",0x7f7f7f7f);
    return 0;
}
```

这句话完全可以用书上的语句来反驳，这是基础不扎实的表现

conversions 转化在 youtube可以用 `www.convyoutube.com/dsfadfnjnkfn(只是一个示例不可访问)`



### 					Other Integer Types

> explicit 反义词 implicit  明显的/直接的 vs. 含蓄的



#### 				Declaring Other Integer Types



#### 				Why Multiple Integer Types?

>this allows integers (in excess of/greater than) 2 billion($2\times10^9$)

> implementers=implementation 工具 仪器

>In principle, 原则上/原理上

> legibility = read-ability 

who's counting? 谁在数呢?

> odometer 里程表

> keep tabs on that.  =  take care of that



#### 				:star:long Constants and long long Constants

> Also, some standard C functions require type long values.

:heavy_check_mark:long long int max(long long int x, long long int y)

:x:long long int max(long long int x, int y)

>To cause a small constant to be treated as type long, you can append an l (lowercase L) or L as a suffix

>Add a u or U to the suffix for unsigned long long, as in 5ull or 10LLU or 6LLU or 9Ull.



#### 				Printing short, long, long long, and unsigned Types

>Note that although C allows both uppercase and lowercase letters for constant suffixes, these format specifiers use just lowercase.

%ld %lo %lx

| short   | long    | long long |
| ------- | ------- | --------- |
| 16 bits | 32 bits | 64 bits   |

`int` 在32位机跟long 一样, 在16位机跟short一样, 尽量 少用int 在写有移植需求的工程时,这样便于移植,不用扯皮.但是计算机处理最快的还是int,一个字长.

attribution = property 属性/性质

> truncated

截断 闯脱了头

>it is also your responsibility to use the correct specifier for the type of value to be displayed. :heart:



#### Using Characters: Type char

> punctuation mark

标点符号

>Many IBM mainframes use a different code, called EBCDIC, but the principle(原理) is the same.

> encompass= surround

> initiative = 倡议 = 初步行动

> as far as = 据...而言
>
> >The C language defines a byte to be the number of bits used by type *char*, so as far as C documentation goes, a byte would be 16 or 32 bits,
>
> C语言将字节定义为char类型使用的位数，因此就C文档而言，字节将为16或32位(在用Unicode 字符集的计算机上) byte 也是可以定义的不是一直为8bits:warning:

#### Declaring Type char Variables



#### Character Constants and Initialization

> wind/wound up with = 切开并拿走



#### Nonprinting Characters

>`'\?'`
>
>`'\\'`
>
>`'\"'`
>
>`'\''`

#### Printing Characters

>Recall that a character variable is stored as a *1-byte integer value*(真象).

> 传给print的参数会自动转化为int型的位数,所以%d打印%c的值不会打出奇奇怪怪的值...

> ampersand->&

prompt = call

#### Signed or Unsigned?



#### The _Bool Type

> defer = postpone



#### Portable Types: `inttypes.h`

> adequate number = sufficient 足够数量的

操作系统真象还原的头文件

> synonym or alias

同义词或别名

> designation = appointment 分发/分派 *exact width types* 严格(确定)宽度类型

> get around = overcome

> incidentally = by the way

> rundown = summary
>
> vendors = 供应商

---

下面是浮点数了:bulb:

### Types float, double, and long double(15pages remain->85)

> *scientific notation*科学计数法

> represent at least six significant figures

表示6个有效小数/准确数字

>called the *mantissa* or *significand*, and its sign. 阶码+尾数

双精度型double 精确到小数点后10位 (C标准规定的)最少的

但64位的double implementation 达到了13位的精度 

比float多出的32位全部用来表示尾数(一般是这么实现)表示阶码8位就足够大了10^301次方...

long double 的精度要求和 double 一样在C99标准中,可以理解为4精度型float...

:bulb:真象还原C浮点数​

> round-off errors. 摄入错误

> accommodate = 提供住宿 contain 容纳

#### Declaring Floating-Point Variables



#### Floating-Point Constants

> leave out = omit = 不留下

> the compiler assumes floating-point constants are double precision.

> override = 覆写/废除/不使用
>
> base 10 notation 10进制计数法



#### Printing Floating-Point Values

>If your system supports the C99 hexadecimal format for floating-point numbers, you can use a or A instead of e or E.

这个真可以尝试一下在编程中

>That's because C automatically expands type float values to type double when they are passed as arguments to any function, such as printf()



#### Floating-Point Overflow and Underflow

>but now C specifies that toobig gets assigned a special value that stands for *infinity* and that printf() displays either *inf* or *infinity*(宏定义了的 最大阶码值) (or some variation on that theme) for the value.

> *subnormal* 次正规值

>The C library now provides functions that let you check whether your computations are producing subnormal values.

:arrow_up:挖的这个坑,我希望你能填

可以用%d 输出float 吗 例如printf("%d",(int)3.33333f);

#### Complex and Imaginary Types

> with some reservations.

有所保留的拥护，复数的实现。

### Beyond the Basic Types

> smuggled = 走私

### Type Sizes

> leaves some latitude 

留有余地



## Using Data Types

sloppy = poor = 邋遢/马虎



## Arguments and Pitfalls

> amplify

=enlarge

> tuna 金枪鱼罐头

> finiky = picky = fussy



## One More Example: Escape Sequences

>contemporary graphical interfaces. (现代图形界面)



### What Happens When the Program Runs



### Flushing the Output

>flush = 冲洗

> Every now and then 
>
> 时不时的sometimes but not very often

> impending input

即将来临的=coming

> impending input flushes the buffer

即将到来的输入(导致了)冲洗缓冲区

## Key Concepts

> identical = same 

## Summary



## Review Questions



## Programming Exercises