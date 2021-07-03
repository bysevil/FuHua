# 从Hello World开始学java

## 作为惯例让我们先编写一个最简单的程序*Hello World！*（代码如下），并将它命名为*Hello.java*。

```java
public class Hello{
   public static void main(String[] args){
      System.out.print("Hello,World!");
   }
}
```

#### 值得注意的几点是：

  - 1. 文件名必须与它的类名，即上方程序中的**public class**后面的字符相同，否则程序运行时会报错。

  - 2. 上方程序每个字符都不能有差别，包括空格字符。否则会报错。

  - 3. 字母的大小写不能出现差别，否则会报错。

  - 4. 建议使用英文（包括打印内容），否则有可能会报错。

  - 5. 必须使用英文符号

### 1.如果要运行这个程序，我们需要对这个java文件进行编译：

  - 1. 打开cmd

  - 2. 进入你所储存Hello.java的目录（我的存储目录为*C:\Users\Administrator\Desktop\study*）

  - 3. 输入**javac Hello.java**

如我将输入

```Dos
C:\Users\Administrator\Desktop\study>javac Hello.java
```

   - 如果你的环境没有配置好，或者文件编写有错误，此时会报错

- 如果出现
```Dos
C:\Users\Administrator\Desktop\study>javac Hello.java
'javac'不是内部或外部命令，也不是可运行的程序或批处理文件。
```
   - 则说明你的环境配置出现问题。

- 如果时其他报错提示，那就是你的文件编写有错误，参考上方注意事项

### 2. 此时如果出现以下界面（以我为例）:

  ```Dos
C:\Users\Administrator\Desktop\study>javac Hello.java

C:\Users\Administrator\Desktop\study>
  ```
- 那么恭喜你，编译成功。你的前几步都没有出现问题

- 此时在你存放**Hello.java**的文件夹将会出现一个新文件**Hello.class**

- 这个文件即为编译后的文件（如果没有出现此文件，那么恭喜你，遇到了人生中的第一个BUG）

### 3. 此时在进入此目录的cmd中输入*java Hello*，将运行这个文件

  - 如我将输入
```Dos
C:\Users\Administrator\Desktop\study>java Hello
```

  - 此时cmd将回馈
```Dos
C:\Users\Administrator\Desktop\study>java Hello
Hello,World!
C:\Users\Administrator\Desktop\study>
```
### 如果以上步骤都已完成，那么你成功的编译并运行了*Hello.java*这个代码的编写

## 此时，我们来尝试简单理解这段代码

```java
public class Hello{
  public static void main(String[] args){
    System.out.print("Hello,World!");
  }
}
```

1. **public class**表示一个类，其后面的Hello为类名

2. **public static void**是一段修饰语，我们现在不需要了解它的意思

3. **main**是一种java的一种主方法，即main方法

4. **String[] args**为参数，很显然，这段代码并没有用到参数，即参数为**[空]**

5. **System.out.print**这段字符表示输出，即输出后面的Hello World！