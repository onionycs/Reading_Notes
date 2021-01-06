# toc

[toc]

这一章开始读的是C_primer_plus 第六版

# Operators, Expressions, and Statements

> multitudinous = numerous
>
> Operator precedence = 运算符优先级/priority

> Compound statements = 复合语句

> typecast is a word not two words means 类型转换
>
> addition, subtraction, multiplication, and division. 加减乘除法



## &emsp;&emsp;Introducing Loops

> taps(轻拍) the potential of a computer

挖掘计算机的潜力

> condensed version 压缩版本

> proceed = continue to
>
> portion = part 
>
> checkpoint = pass = 关/游戏里的
>
> the extent of = the range of
>
> Centigrade to Fahrenheit 摄氏度to 法润海特
>
> flank = side

## &emsp;&emsp;Fundamental Operators



### &emsp;&emsp;&emsp;&emsp;Assignment Operator: = 

> hair-splitting = 头发分裂 crack/divide
>
> modifiable lvalue = 可修改的左值
>
> the most intuitive phrase you’ve encountered 您遇到的最直观的短语
>
> Some Terminology: Data Objects, Lvalues, Rvalues, and Operands
>
> 一些术语：数据对象，左值，右值和操作数
>
> For example, you could specify an element of an array, a member of a structure, or use a pointer expression that involves the address of the object.
>
> 例如，您可以指定数组的元素，结构的成员，或使用涉及对象地址的指针表达式。
>
> referred to = mentioned
>
> object locator value = 对象定位器值
>
> In the context of = 在···的背景下
>
> context means situation
>
> as long as 只要
>
> flashier = impressive
>
> golf tournament scorecard = 高尔夫比赛计分卡
>
> Many languages would balk at the triple assignment made in this program, but C accepts it routinely.
>
> 许多语言都  抵制/不情愿/抵触  接受此程序中的三重分配，但是C 例行/常规地 接受它。
>
> 

### &emsp;&emsp;&emsp;&emsp;Addition Operator: + 

> bribe = 贿赂
>
> 

### &emsp;&emsp;&emsp;&emsp;Subtraction Operator: – 

> binary , or dyadic, operators = 双目运算符
>
> 

### &emsp;&emsp;&emsp;&emsp;Sign Operators: – and + 

> algebraic sign = 代数符号
>
> unary operator = 单目运算符

### &emsp;&emsp;&emsp;&emsp;Multiplication Operator: * 

> By any chance, do you want a table of squares? 碰巧,你想要一个平方数表格吗
>
> lacking mathematical erudition = knowledge
>
> erudite = learned
>
> astounded at the modesty of this request = 对此要求的谦虚感到震惊
>
> astonished 吃惊  = astounded
>
> Because you might not be **up to date** on wheat crops, the program also compares the **running total** to a very rough estimate of the annual world wheat crop.
>
> 由于您可能不了解最新的小麦作物，因此该程序还会将**运行总量**与对世界年度小麦作物的非常粗略的估计进行比较。
>
> haul = transport = 运输量 a haul of antiques 一般来说不合法的东西
>
> 

### &emsp;&emsp;&emsp;&emsp;Division Operator: / 

>give some leeway to 给```留有余地
>
>The properties of integer division turn out to be handy for some problems, and you’ll see
>an example `fairly soon`.
>
>

### &emsp;&emsp;&emsp;&emsp;Operator Precedence 

> pecking order 啄食顺序
>
> The associativity column 关联列

### &emsp;&emsp;&emsp;&emsp;Precedence and the Order of Evaluation 



## &emsp;&emsp;Some Additional Operators 



### &emsp;&emsp;&emsp;&emsp;The sizeof Operator and the size_t Type 

the _t means type so size_t means size type    size类型  typedef unsigned size_t

### &emsp;&emsp;&emsp;&emsp;Modulus Operator: % 

> esoteric tool 深奥的工具
>
> bill-preparing 账单准备
>
> Before C99 settled on the “truncate toward zero” rule for integer division, there were a couple of possibilities.
>
> you get a negative modulus value if the first operand is negative, and you get a positive modulus otherwise
>
> if a and b are integer values, you can calculate a%b by subtracting (a/b)*b from a .

### &emsp;&emsp;&emsp;&emsp;Increment and Decrement Operators: ++ and -- 

> give your programs an elegant gloss
>
> 光泽/cover
>
> merit = worth
>
> compensate 补偿
>
> The computer would churn out line after identical line
>
> 计算机将在同一行之后逐行输出 搅拌
>
> dread = scaring
>
> delicate = 精巧 = subtle 
>
> dictate = command

### &emsp;&emsp;&emsp;&emsp;Decrementing: -- 

> lyricist 作词家
>
> accomplished = elegant
>
> 

### &emsp;&emsp;&emsp;&emsp;Precedence 



### &emsp;&emsp;&emsp;&emsp;Don’t Be Too Clever 

`printf("%10d %10d\n", num, num*num++);`

it might evaluate the last argument first and increment num before getting to the other argument.

the compiler can choose which arguments in a function to evaluate first. This freedom increases compiler efficiency, but can cause trouble if you use an increment operator on a function argument.

You can easily avoid these problems:
■ Don’t use increment or decrement operators on a variable that is part of more than one
argument of a function.
■ Don’t use increment or decrement operators on a variable that appears more than once
in an expression.

use them,inc or dec them, 使用他们两侧,这个use them的条件就模糊不清了.



## &emsp;&emsp;Expressions and Statements 



### &emsp;&emsp;&emsp;&emsp;Expressions 

赋值表达式的值等于 modified lvalue 的值



### &emsp;&emsp;&emsp;&emsp;Statements 

> workhorse 主力
>
> That means all changes made by assignment operators, increment operators, and decrement operators in a statement must take place before a program proceeds to the next statement
>
> Now consider this statement:
> y = (4 + x++) + (6 + x++);
> The expression 4 + x++ is not a full expression, so C does not guarantee that x will be incremented immediately after the subexpression 4 + x++ is evaluated. Here, the full expression is the entire assignment statement, and the semicolon marks the sequence point, so all that C guarantees is that x will have been incremented twice by the time the program moves to the following statement. C does not specify whether x is incremented after each subexpression is evaluated or only after all the expressions have been evaluated, which is why you should avoid statements of this kind.

### &emsp;&emsp;&emsp;&emsp;Compound Statements (Blocks) 

> indentation 缩进

## &emsp;&emsp;Type Conversions 

> inadvertently 不经意地
>
> advertent 故意
>
> uneventful 平稳的 / 没有很多事件发生,很平稳

### &emsp;&emsp;&emsp;&emsp;The Cast Operator 

>  steer  clear of = drive to avoid
>
>  This is the general form of a cast operator:
>  ( type )
>  The actual type desired, such as long , is substituted for the word type
>
>  intrinsically = in essence
>
>  The C philosophy is to avoid putting barriers in your way and to give you the responsibility of not abusing that freedom.
>
>  Miscel-laneous 其他的 杂

## &emsp;&emsp;Function with Arguments 

在函数传参过程中的类型转化。

prototype -》an implicit type cast in the function call



## &emsp;&emsp;A Sample Program 

》for a narrowly defined subgrouping of humanity

对于人类的狭义分组

>The bulk of = most part of  the program relays = conveys information between the computer and the user.

> metric  以米计数的



## &emsp;&emsp;Key Concepts 



## &emsp;&emsp;Summary 



## &emsp;&emsp;Review Questions 

> What makes this design inferior to the original?

是什么使该设计不如原始设计？

## &emsp;&emsp;Programming Exercises 



