# java学习笔记

## java的特性

1.java是面向对象的语言 两个要素：类和对象 三个特征：封装继承多态
2.Java是具有健壮性的 去除了c语言的指针；自动的垃圾回收机制；仍然会内存溢出，内存泄漏
3.java语言是跨平台性的
4.java语言是解释性的（解释性语言）

JDK>JRE>JVM

JDK=JRE+java的开发工具（javac java javadoc）

JRE=JVM+java的核心类库

java的引用数据类型：**类（string）在java中双引号括起来的**   **数组  接口**

## java编译和运行

1.java的编译 使用javac 文件名.java

2.java的运行 java 文件名

## 细节功能

在控制台 按下**tab**键可以实现命令的补全
\t实现对齐的功能
\n实现换行的功能
在字符串中要输出双引号要使用转义字符 \
\r 代表回车
整形的细节：声明long之后的常量要加l或者L；
浮点数：float有4个字节
              double有8个字节
java的浮点型默认为double 声明float要在数字的后面加上”f”或“F”

## 文档的编写

**格式**：/**  

 @author 指定java程序的作者

 @version 指定源文件的版本 

 */

**操作方式**

**javadoc -d (起一个文件夹的名字)-author-version (文件名).java**
文档注释可以被jdk内置的javadoc所解析，生成一套以网页形式体现的该程序的说明文档

打开有个index.html的文件
在一个java源文件中，可以声明多个class但是最多只能有一个类声明为public，而且要求声明public的类名称必须与源文件名相同。

## java的基础操作

### 输入输出

**输入**：java从键盘输入数据：
1：**导入Scanner类**
import java.util.Scanner；
2：**创建Scanner对象**
Scanner scan =new Scanner(System.in);
3:从键盘上获取用户输入的数据
String/int/double/has num=scan.next()/.nextInt()/.nextDoube()/hasnext();
注解：
input.next()：获取一个字符串；
input.nextInt()：获取一个整数；
input.nextDoube()：获取一个双精度浮点数；

**输出**：

System.out.println();先输出数据，然后换行
System.out.print();只输出数据，不换行

## swich和while注意事项

1.swich语句要和break来搭配使用
   swich语句的条件不满足布尔类型：只能是如下六种：byte  short  char  int 枚举类型 string类型；

2.while循环的注意事项

条件1
while(条件2)
{条件3；
条件4；
}

3.break和continue的使用辨析：

break使用在swich语句和循环语句；continue在循环中使用；

break使用时是结束**当前**循环,continue的使用是结束**当次**的循环；

break和continue后面不能跟其他的语句。

## 数组

1. 数组首先要定义

2. 数组的数据类型必须是一致的

3. 数组是连续排列的

4. 数组要注意界限 存储的元素个数不能多于数组的大小 防止发生数据的溢出

5. 数组会开辟出一块连续的空间

数组的初始化：

int[num]

数组的静态初始化：

Num=new int[ ]{1,2,3,4}

数组的动态初始化：

String[ ] num=new String[5]

数组完成了初始化，那么数组的长度就确定了

**如何获取数组的长度：**

属性：**length**

```java
System.out.println(names.length)//使用length属性来计算代码的长度
```



























