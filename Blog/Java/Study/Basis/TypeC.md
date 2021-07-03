# java类型转换
1. **java是强类型语言，所以有些运算需要用到类型转换**
2. ***运算中，不同类型数据转换为同一类型，再进行运算***
3. 从低到高转换
byte,short,chat->int->long->float->double
***浮点数类型始终高于整数类型***
## 强制转换
```java
    int i = 126;
    byte b = (byte)i;
```
- 这串代码将一个int类数据转换为了byte类
- 由于是由高到低转换，这属于强制转换
***强制转换的时候可能存在内存溢出或者精度不够***
## 精度不够
```java
        float f = 12.3f;
        int i1 = (int)f;
```
输出时f为12.3，i1为12，精度不够
## 内存溢出
```java
    int money = 10_0000_0000;
    int year = 20;
    int total = money*year;//因为int类只占4个字节，所以造成了内存溢出
    long total2 = money*year;//使用更高级的long类同样，因为java是默认先运算在转换，所以已经存在了内存溢出
    long total23 = money*((long)year);//此时输出正常，因为我们先强制转换再运算
```
## 自动转换
```java
        int i3 = 126;
        double b2 = i3;
```
在从低到高转换时，系统会自动转换
## 在数据转换中，我们需要注意
- 数据转换不能涉及布尔值
- 不能把对象类型转换为不相干的类型
