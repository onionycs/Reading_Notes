# 吐槽

　　1.要警惕IBM陷阱，学什么东西切记不要有一下学完的想法，应该遵循事务发展的基本规律。

`Wave forward spiral upward。`

　　2.坚持保持更新自己的软件是个好的习惯,没了jobs的:apple:公司下作的行为让程序员不齿,所以要爱护自己的源码,爱护自己的repository.

　　3.读英语原版书的还有一个好处是看到自己学过的知识时也不会觉得无聊,因为里面有很多不认识的单词:laughing:  just found I obfuscate the two words, image and [emoji](https://gist.github.com/rxaviers/7360908#file-gistfile1-md), respectively. :joy:

　　4.做人不要慷他人之慨,不是你的你没有任何操控和伸手的权利!:anger:



# Chapter 2. Introducing C

> put together

`==放在一起==build`

> integer-valued

`整数值的/整数型的 加ed只是为了变成形容词`

> newline character

`换行符`

> skim through

`==scan==browse`

> quite likely

`very perhaps/maybe`

> C looks a little peculiar

`abnormal==strange`

> sprinkled with symbols

==spread

`If something(source code file) is sprinkled with particular things, it has （a few of）=many them(symbols) throughout it and they are far apart from each other.`我们中 遍布many 了异类 

> characteristic C symbols

`特有的/独享的`

整段内容是用skim through 和 read through 两种过程形成对比

## A Simple Example of C

> Exactly

`究竟,到底 very`责问的语气

> apparent

`==obvious`

> all in all

`总之`

## The Example Explained

> We'll take two `passes` / through the program's source code.

`==check point 关(in the radio game)` ex. Pass 1 means 第一关

> Synopsis

`==summary`

> highlights the meaning

verb. 强调 突出 `==stress`

> specific implications

`==meaning` implement实现

> anatomy

`==analyse/examination`

长期以来的翻译错误

> preprocessor instructions

这是预处理器指令，不上处理器的指令，给compiler看的

> building blocks

`==module`模块组件 也可翻译成积木toy bricks

> statements

语句

> identifier

标识符

### Pass 1: Quick Synopsis

> topics raised here

`==questions`

> identify

`==determine确定（身份）==evaluate鉴定==appraise(评价)`

>something more recent to avoid incompatibilities.

一些更靠近 远离不兼容可能的 东西

> enclose comments, remarks 同位语从句还是定语从句呢？修饰还是解释说明不好判断
>
> 好判断的是从句缺不缺成分却成份就是定语从句，that是先行词/引导词
>
>  that help clarify a program

`==hug==surround==embrace` 

>are intended

`are planned`

>It's termed

`被术语 jargon`

> tacks on

verb. `==append==add to` noun. `大头钉`

> furnish

`==provide`

> agency

`==mechanism机构`

### Pass 2: Program Details

#### `#include Directives` and Header Files

`==instructions`

> In effect, it's a cut-and-paste operation

> preparatory

adjective. prepare

> stands for

`==represent`

> Incidentally

`meantime==by the way`

#### The main() Function

> proclaims

pro means forward(before a crowd) so proclaim means announce 宣布

> The C90 standard grudgingly$\downarrow$ tolerated this form,

勉强忍受 reluctantly grudge（hate）

> confine `==limit`

> C99 adds a second style of comments, one popularized by C++ and Java.

是第二种不是两种。第一次读理解错了造成了较大的误会。这个地方就是同位语从句

### Braces, Bodies, and Blocks

> delimit `==limit the area`

定界

>Their presence is mandatory, so don't leave them out.

`他们的存在是强制性的,所以不要将他们排除在外`

#### 现在才发现打中文可以使用英语符号这样可以很好的打出一些markdown的标记

`mandate==order==command==claim(要求)`

>Only braces ({ }) work for this purpose, not parentheses (( )) and not brackets ([ ]).

明确了几个括号的表达方式, 大括号,圆括号,方括号

### Declarations

> usurp$\downarrow$ them for other purposes

force

>may void this option in some locales.

`使无效化`

> *identifier* in C refer to 变量名\函数名\结构体名等统称的标识符

> the practice of C++  (fact way)实际方法

#### Data Types(use Ctrl+4 to rank)

> investigate

`检查鉴定 评价(appraise)`

#### Name Choice

> doesn't suffice

fulfill/satisfy (合格/满足)

> Documenting a program `==codify/organize`

> techniques==skills

>Storage `Classes`, Linkage, and Memory Management 存储类

>the compiler won't pay attention to the extra characters. Therefore, on a system with an eight-character limit, `shakespeare` and `shakespencil` would be considered the same name

> concoct==fabricate  `编造`==prepare`准备`

> virtual city 虚拟城市   fabricated city虚构的城市

>Operating systems and the C library often use identifiers with one or two initial underscore characters, such as in `_kcab`, so it is better to avoid that usage yourself.

`__starts__ ` two underscore before starts

retain强调的是放在那里别动它,reserve 强调的是藏起来,别动它,保留

> C names are *case sensitive*

supper case/lower case sensitive

the word use italic font means a jargon/term

#### Four Good Reasons to Declare Variables

> plunging into writing a program

dive/jump into 潜入/跳入 verb. plunge

>helps prevent one of programming's more subtle and hard-to-find bugs

`secret and gentle` 隐秘而微小ultra-fine的

> circumference == 周长

`==perimeter`

> unwittingly

`==unconsciously`

> wittingly or unwittingly

有意(故意liberate `liber的 intentional/on purpose`)无意地

> preceding/precedent pre means pro 

former/former instance

> C prior==former standard C90

### Assignment

> assign==分配 distribute

> set aside  `pre divide` 预留 `gash 划开`

### The `printf()` Function

> actual argument

实参

> 主调函数==*the calling* function

> 换行符==*newline character*

> far-left means 最左

> 转义序列==*escape sequence*
>
> backslash==反斜杠 \\

> oddity is a noun means peculiar person/thing like the word wack

> recall is like remind by yourself/ remember once again

> review of substitute : it's meaning == replace

> symbol group %d 符号对儿

> *formatting* print function--> `printf`

> specifier 说明符 ex. decimal -->%d --> integer

### Return Statement

> chide == scold/curse

> logical consistency == 逻辑上的一致性/conformity



## The Structure of a Simple Program

> recognize==determine==identify

> terminate 终结 terminator 终结者

## Tips on Making Your Programs Readable

> practice (specific/current way)

> two techniques complement each other两种技巧互为补充

> video routine 视频(fixed) 程序

> hyphen 连字符 read-ability

> legitimate==legal

>As adjectives the difference between **legal** and **legitimate**  is that **legal** is relating to the law or to lawyers
>
> while **legitimate** is in accordance with the law or established legal forms and requirements; lawful.

> fathom is a length unit. 6 feet equal to 1 fathom.

## Taking Another Step in Using C

### Listing 2.2. `The fathm_ft.c` Program

### Documentation

### Multiple Declarations

### Multiplication(verb. multiply)

> harness==drive/mount(mount 有安装install的意思)

### Printing Multiple Values

> fancy means 花式的(:+1:)==excellent

## While You're at It—Multiple Functions

### Listing 2.3. The `two_func.c` Program

> butler means 男管家/男仆 rang (a bell) 摇铃/按铃

>The first appearance is in the *prototype*, which informs the compiler about the functions to be used. 函数原型(声明declaration)==FUNCTION DECLARATION

> in turn == one by one 轮流

> in a moment == soon `很快啊`



## Introducing Debugging

### Listing 2.4. The `nogood.c` Program

### Syntax Errors

> analogous

adjective. `similarity`

> alternatively

`==or  alternative==other/another`

> a line late. 

postpone/put off one line >check the line before.佐证

编译器报告syntax 错误会推迟一行

> deduce==conclude

### Semantic Errors(语义logic 错误)

> violate C rules.

### Listing 2.5. The `stillbad.c` Program

> cube-wise 立方体( manner or extent )

> wound up with 

==wind up with (past and past participle of wind)==result in

> in this fashion=way

### Program State

> feel up=satisfied to

> illuminate=lighten

> Debuggers come in various levels of ease of use and sophistication.
>
> 调试器具有各种易用性和复杂程度。

> handy=convenient

> alternative=different



## Keywords and Reserved Identifiers



## Key Concepts

> attention=keep mind on

> underlying底层的

## Summary

> consist=constitute
>
> the called function被调函数

## Review Questions

## Programming Exercises

