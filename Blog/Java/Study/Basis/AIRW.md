# java注释和标识符

## java注释
![^1]:java注释不会被程序运行，它只是为了阅读者更好的理解这段程序
1. 单行注释
```java
   //这是一个注释
```
2. 多行注释
```java
   /*这是一个注释
     并且涉及多行
   */
```
3. 文档注释
```java
/**
 * @Description
 * @Auther 
 */
```
## java 标识符
### 标识符
 1. java所有的组成部分都需要有名字，类名，变量名以及方法名都被称为标识符。
 2. 所有的标识符都应该以字母(*A-Z*或*a-z*)，美元符(*$*),或者下划线(*_*)开头
        - 首字母之后可以是任何字符（大小写字母，美元符，下划线等)组合（但是不要使用特殊符号如*#* ，*%*）
 3. 不能使用关键字作为变量名或者方法名
 4. 标识符是大小写敏感的(即A与a是两个变量名)
 5. 可以使用中文命名，但是不建议
 6. 变量不能重名