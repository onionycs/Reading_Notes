[toc]



56.23% 

可复制的pdf版本唯一的不好就是在复制过后的粘贴会自动的断行

# 13 File Input/Output 

correspondence = letter

myriad = a countless or extremely great number.

## Communicating with Files 



### What Is a File? The Text Mode and the Binary Mode 

说这么多各式各样的file format 就是为了证明C很吊吧。

regularity 规律性。

nautical
of or concerning sailors or navigation; maritime.



### Levels of I/O 



### Standard Files



## Standard I/O 

这三节的文字很多，比较难理解，果然C才是简单的。
读的太痛苦了，这些文字。



### Checking for Command-Line Arguments 

涉及文件的部分需要很多的操作系统的知识，比如FILE* 类型指向的究竟是个啥？

![](.\images\FILE.jpg)



### The fopen() Function 



### The getc() and putc() Functions 



### End-of-File 



### The fclose() Function 



### Pointers to the Standard Files 



## A Simple-Minded File-Condensing Program 



## File I/O: fprintf(), fscanf(), fgets(), and fputs() 



### The fprintf() and fscanf() Functions 

所以a模式,r模式的区别在哪里呢? 我rewind a模式(非a+)的话可不可以读出东西呢? 还是说所有get的函数都不能用了呢?

### The fgets() and fputs() Functions 



## Adventures in Random Access: fseek() and ftell() 



### How fseek() and ftell() Work 



### Binary Versus Text Mode 



### Portability 

总的来说C处理文件还是有很大的弊端,比如说有年代感,毕竟是1978年的古董,原生的支持大多只针对text file 而且还是UNIX和MS-DOS系统的文件,到现在不适用也很正常. 大概了解一下,甚至不了解也可

C对UNIX和LINUX的text文件支持的最好(不用做那么多map)

The C preprocessor conditional compilation directives:star:



### The fgetpos() and fsetpos() Functions 



## Behind the Scenes with Standard I/O 



## Other Standard I/O Functions 



### The int ungetc(int c, FILE *fp) Function 



### The int fflush() Function 



### The int setvbuf() Function 



### Binary I/O: fread() and fwrite() 



### The size_t fwrite() Function 



### The size_t fread() Function 



### The int feof(FILE *fp) and int ferror(FILE *fp) Functions 



这一章就看到这把，太不好看了。最后两个例子一点也不好读。

### An fread() and fwrite() Example 



### Random Access with Binary I/O 



## Key Concepts 



## Summary 



## Review Questions 



## Programming Exercises 





