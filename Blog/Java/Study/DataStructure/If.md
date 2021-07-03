# if选择结构

首先我们要知道，java的基础数据结构是顺序结构

> if语句可以没有else，可以只有一个if

## 1.if单选结构

```java
if(name.equals("Hello")){
    System.out.print("World")
}
```

此时如果name的值为Hello，则会运行代码，输出"World".

> equals是一个比较字符串是否相等的语法

## 2.if双选择结构

```java
if(name==1){
    System.out.print("你输入了数字1")
}else{
    System.out.print("你输入的不是数字1")
}
```

此时如果name的值为一，运行第一段代码，否则会运行第二段代码

## 3.if多选择结构

```java
if(name==100){
    System.out.print("满分")
}else if(name>=0&&name<=100){
    System.out.print("非满分")
}else{
    System.out.print("非法的成绩")
}
```

此时会按照你输人的数字判断你的成绩区间

## 4.if嵌套结构

```java
if(name>=0&&name<=100){
    if(name>=60){
        System.out.print("及格")
    }else{
        System.out.print("不及格")
    }
}
```

我们可以在一个if里嵌套另一个if，这在其他数据结构里也适用