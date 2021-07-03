# Scanner对象

- 通过Scanner我们可以获取到人的输入

### 1. 基本语法：
```java
Scanner name = new Scanner(System.in);
```
  这样我们创建了一个扫描器对象，用来获得用户输入
### 2.判断用户有无输入
```java
if(name.hasNext()){
    System.out.print("如果用户有输入打印这段话")
}
```
- 我们一般使用hasNext（）与hasNextLine（）判断是否还有输入的字符。
### 3.接收用户输入
```java
String name1=name.next()
```
将用户name的输入赋值给name1
我们一般使用next()和nextLine()方式接受用户输入，区别在于
- next()以空白键或者回车键为结束，无法输出空白以后的内容，而且只有在输出有效字符后才能结束
- nextLine()只以回车键为结束，可以获得空白
### 4.在用完之后关掉这个类
```java
name.close()
```
凡是属于IO流的类，用完后必须关掉
## 现在我们学习一些进阶操作

### 1. 我们依然是先创建一个扫描器对象，读取用户输入

```java 
Scanner scanner = new Scanner(System.in);
```
### 2. 接下来进行一些进阶操作

```java 
    int i = 0;
    float f = 0.0f;
    System.out.println("请输入整数：");
    if(scanner.hasNextInt()){//如果用户输入了一个整数，运行下面代码（以nextLine方式接收）
       i = scanner.nextInt();//使i=用户输入
       System.out.println("整数数据："+i);//输出i
    }else{//否则（即当用户输入的不是整数时），运行下面代码
      System.out.println("你输入的不是整数数据");
    }
    System.out.println("请输入小数：");
    if(scanner.hasNextFloat()){//如果用户输入了一个小数，运行下面代码（以nextLine方式接收）
      f = scanner.nextFloat();//使f=用户输入
      System.out.println("小数数据："+f);//输出i
    }else{//否则（即当用户输入的不是小数时），运行下面代码
      System.out.println("你输入的不是小数数据");
    }
    scanner.close();//关闭这个代码
```
- 对于上面的代码我们发现，如果第一次输入为整数，则会返回这个数，然后进入下一段代码（即小数代码）
- 而如果你在第一段代码直接输入了一个小数，则会返回”你输入的不是整数“，然后下一段代码直接返回这个小数
***总结，第一个判断错误后直接跳过输入判断第二个***
- 我们可以判断任何类型的字符串以运行相应代码
## 现在我们对于上面学到的知识进行一个简单应用
```java
package ProcessControl;
import java.util.Scanner;
public class Scanner3 {
  public static void main(String[] args){
​    Scanner scanner = new Scanner(System.in);
​    System.out.println("请输入一个数字");
​    double x = 0;
​    int m = 0;
​    while(scanner.hasNextDouble()){
​      m=m+1;
​      x = x+(scanner.nextDouble());
​      System.out.print("这是你输入的第"+m+"个数据,");
​      System.out.print("此时所有输入的数据和为:"+x);
​      System.out.print(",平均数为:"+(x/m));
​    }
​    scanner.close();
​    System.out.println("==============over=========");
​    System.out.println("你总共输入了"+m+"个数据");
​    System.out.println("它们的和为"+x);
​    System.out.println("平均数为"+(x/m));
  }
}
```
我们创造了一个计算器，计算用户输入数据的和与平均数。
