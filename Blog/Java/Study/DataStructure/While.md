## While循环结构

#### while是最基本的循环，它的结构为

```java
int i = 0；
while(i<100){
    i++;
    System.out.println(i)
}
```

当i<100成立时会不停运行while里的内容，直到其不成立

那么，如果i<100始终成立呢？

#### 那被称为死循环，如

```java
int i2 = 0;
while(i<1){
    System.out.println(i)
}
```

这个程序会一直运行

## Do...While循环

- 在while循环中，如果布尔表达式始终不成立，则不会运行while循环里的内容。

此时，如果我们想要其即使表达式不成立也要使程序至少运行一次则要使用Do..While循环

```java
int i3=2
do{
    System.out.println(i3)
}while(i3<1)
```



