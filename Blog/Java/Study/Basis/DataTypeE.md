## 整数扩展
在java中，整数不仅可以用十进制，也可以用其他进制
如
#### 二进制(以0b开头）
```java
int num1 = 0b10
```
这样将会输出2
#### 八进制0
```java
int num2 = 010
```
这样将会输出8
#### 十六进制0x
```java
int num3 = 0x10
```
这样将会输出16

## 浮点数扩展
float double 是有限的离散的，有舍入误差（即结果会四舍五入）在直接输出时不会影响，但在运算中会使得输出结果与实际结果有误差）
例如
```java
float num1 = 0.1f
float num2 = 1/10f
System.out.println(num1==num2)
```
在数学上我们知道0.1=1/10成立即num1=num2为真(true)
但是如果你运行这个java程序，将出现
```java
0.1
0.1
false
```
这便是舍入误差的影响
再举一个例子
```java
float num1 = 1203810f
float num2 = num1+1
System.out.println(num1=num2)
```
在数学上，1203810+1显然不等于1203810，但输出时我们发现返回结果为true
所以**最好完全避免使用浮点数进行比较**

>那么我们要如何运算呢
>使用BigDecimal类进行运算 这是一种数学工具类

## 字符扩展
首先我们要了解到，在计算机中，所有的**字符本质都还是数字**。
现在我们使用***强制转换来使一个字符转换为数字
```java
char c1 = "a"
char c2 = "中"
System.out.print(c1)
System.out.print(c2)
System.out.print((int)c1)
System.out.print((int)c2)
```
此时会输出
```java
a
中
97
20013
```
我们将字符转换成了数字，这便是强制转换
同样的，我们也可以将数字转换为字符
```java
char c3 = 'u10061'
```
此时如果输出c3，系统将返回*a*
>这是Unicode编码的表示方式
## 布尔值扩展
我们定义一个布尔值
```java
boolean flag = true;
```
在使用if
```
if (flag==true) {}
```
这行代码可以使的flag=true时运行一段代码，flag=false时不运行这段代码
但是实际上，使用
```java
if(flag){}
```
可以达到同样效果，因为它的默认值为true
