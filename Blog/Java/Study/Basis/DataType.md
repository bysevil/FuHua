# java的8大基础数据类型

> java是强类型语言，要求变量的使用严格符合规定，所有变量必须先定义才能使用。
> 非8大基础数据类型的，都属于引用类型

## 整数类型

```java
byte num1=10;
```
byte类型在整数里最常用，占一个字符范围，即从128到127

```java  
short num2=20;
```
short类型占两个字符范围，即从-32768到32767

```java  
int num3=30;
```
int类型占四个字符范围，即从-2147483649到2147483648

```java
long num4=40L;
```
long类型占8个字节范围***（后面要加L)***，即从-9223372036854775808到9223372036854775807

## 浮点数类型（即小数）

```java
float num5=50.1F;//
```
float类型占4个字符，****后面加F****

```java
double num6 = 3.1415926;
```
double类型占8个字符



## 字符类型

```java
char name = "A"//
```
char类型的值只能是一个字符

## 字符串类型
```java
  String name1 = "bysevil"
```
String类型可以是多个字符，表示一个字符串，***（String不是保留字）***



## 布尔类型

```java
boolean flag1 = true
boolean flag2 = false

```
布尔值只有“是(true)”“非(false）”两种值，且只占一个位