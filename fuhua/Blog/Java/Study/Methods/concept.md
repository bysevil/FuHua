# 什么是方法

1. **方法**：方法就是行为，一个类可以有很多方法。逻辑运算、数据修改以及所有动作都是在方法中完成的。

- 方法是语句的集合，它们在一起执行一个功能

- 方法是解决一类我的的步骤的有序组合

2. **方法**包含于类或者对象中
3. **方法**在程序中创建

4. **方法名**：所有的方法名都应该以小写字母开头。如果方法名含有若干单词，则后面的每个单词首字母大写。

## 设计方法的原则

方法的本意是功能块，就是实现某个功能的语句块的集合。我们设计方法的时候，最好保持方法的**原子性**，就是**一个方法只完成一个功能，这样有利于我们后期的扩展**

## 方法的的简单设计和调用

```java
public class One {
    public static void main(String[] args) {
        int sum=add(1, 2);//此时我们调用这个方法，并给a，b分别赋值1和2使得sum成为a,b的和
        System.out.println(sum);
        text();//现在我们引用这个方法
    }
    public static int add(int a,int b){//这样我们写出了一个方法
        return a+b;//作用为计算两个int数据a和b的和
    }
    public static void text() {//这是我们之前写过的一个方法
        //作用是打印一个三角形
        int i1=5;
        int i2=5;
        for (int i = 0; i <= 5; i++) {
            for (int j = 0; j <= 10; j++) {
                if(j<=i1&&j>=i2){
                    System.out.print("*");
                }else{
                    System.out.print(" ");
                }
            }
            i1++;
            i2--;
            System.out.println("");
        }
    }
}

```





