# Table Of Contents

1. [Chapter 4. Character Strings and Formatted Input/Output](#Chapter-4.-Character-Strings-and-Formatted-Input/Output)
   1. [Introductory Program](#Introductory-Program)
   2. [Character Strings: An Introduction](#Character-Strings:-An-Introduction)
   3. [Constants and the C Preprocessor](#Constants-and-the-C-Preprocessor)
      1. [Type `char` Arrays and the Null Character](#Type-`char`-Arrays-and-the-Null-Character)
      2. [Using strings](#Using-strings)
      3. [The `strlen()` Function](#The--Function)
      
      4. [Exploring and Exploiting `printf()` and `scanf()`](#Exploring-and-Exploiting--and-)
      5. [Key Concepts](#Key-Concepts)
      6. [Summary](#Summary)
      7. [Review Questions](#Review-Questions)
      8. [Programming Exercises](#Programming-Exercises)

# specified toc

[toc]



# Chapter 4. Character Strings and Formatted Input/Output



## Introductory Program

> engage in =  employ = busy in



## Character Strings: An Introduction



### Type `char` Arrays and the Null Character



### Using strings



### The `strlen()` Function

> The previous chapter unleashed the `sizeof` operator

unleashed = open/set free

> occupy = hold/seize

> The phrase of praise = 赞美用的短语

> how much memory to set aside to store the phrase

set aside to = reserve

> rather trivial purpose of satisfying a user's potential curiosity

满足用户潜在好奇心的相当琐碎的目的



## Constants and the C Preprocessor

> accidentally = occasionally

> manifest constants. = show/obvious

> construction = structure
>
> concern = 关注
>
> niche = room
>
> former(两者中的前者), latter(两者中的后者)

> Difference between 1.00 and the least float value greater than  1.00
>
> 1.00与大于1.00的最小浮点值之间的差



## Exploring and Exploiting `printf()` and `scanf()`

> Exploit

= make use of

> versatile 多才多艺/flexile = flexible = adaptable = useful

### The `printf()` Function

> historically = with reference to past events.  历史上

> historic = famous/important 历史性/重要的(转折)
>
> discrepancy = lack of compatibility/difference

### Using `printf()`

>espresso = black coffee

> thou art too dear for my possessing
>
> 你太珍惜我的财产

> Farewell = bye-bye

> :warning:analogy & anatomy

> **Woe unto you** should you forget this basic requirement

如果您忘记了此基本要求，**您会感到痛苦**

> squid = 乌贼 slug = 铅条/毛虫/懒汉

> If you just want to print data, you can dispense with the running commentary.

如果只想打印数据，则可以省去  正在运行的注释/控制字符串里的除了conversion specification的字符。

dispense = manage without or get rid of.

> bungled = mess up/ fail

> Only 12% of Sally's gribbles were edible. 

sally海的 小害虫 只有12％是可食用的。

> tuck into 塞进



#### Conversion Specification Modifiers for `printf()`

> are still automatically converted to `double`.



#### Examples Using Modifiers and Flags

> authentic imitation! 正品仿制品
>
> blurb 广告

#### Using What You Just Learned



#### :bulb: What Does a Conversion Specification Convert?

> conversion = translate routine



#### :bulb:Mismatched Conversions

> you can say that the number is interpreted modulo  256

模

> does not convert an integer to a floating-point number.

check point

> even the correct specifier can produce phony=false/fake results 

即使是正确的说明符也可以产生伪造的结果

> exact details = accurate detail

> It does so by placing them in an area of memory called the stack. 

32位机传递参数才使用的栈, 因为在C语言中用的int 是(他认为的)计算机字长. 64位个人计算机横行得现在,C语言还是保持了32位的int , 可能是为了兼容性,所以还是利用的栈传参.如果编译器的版本不新...但是CSAPP用的gcc版本足够新,就不是用栈来传递参数了

#### The Return Value of `printf()`

> incidental  = accessary 附带的

返回值是打印的字符数包含看不到的换行符

#### Printing Long Strings



把printf 看完我整个人留下最深印象的是mismatch的部分,因为以前不了解,没有学到过相关的内容

放入栈的时候是按照参数, 取出来的时候是按照 转换说明符

### Using `scanf()`

> inverse = opposite

> :question:Suppress assignment 禁止分配

> it won't discuss the more esoteric features.

深奥的

table 4.6 的%x 和%o 应该是unsigned integer 类型把



#### The `scanf()` View of Input

> versatility  = 通用性

#### Regular Characters in the Format String

> That is, the command `scanf("%c", &ch)` reads the first character  encountered in input, and `scanf(" %c", &ch)` reads the first  non-whitespace character encountered.

regular = 普通的



#### The `scanf()` Return Value



### The `*` Modifier with `printf()` and  `scanf()`

> When placed between the `%` and the specifier letter, it causes that  function to skip over corresponding input.



### Usage Tips for `printf()`

> ragged 破烂的






## Key Concepts

> exert care to 

= unleash = use

> 这里很好的解决了我的sscanf问题
>
> 就是PAT甲级考试的sscanf 问题
>
> 

## Summary



## Review Questions



## Programming Exercises