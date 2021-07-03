# Switch多选择结构

- switch case 语句判断一个变量与一系列值中的某个值是否相等，每个值称为一个分支

- Switch语句中的变量类型可以是byte，short，int或者char（从Java SE7开始支持String）
- 同时case标签必须为字符串，常量或者字面量。

> Switch可以不要break，可以不要default，可以只有一个case

```java
Switch(name){
    case'a':
    System.out.println("优秀");
    break;
    case'b':
    System.out.println("良好");
    case'c':
    System.out.println("差");
    default:
    System。out。println("非法的成绩")
}
```

- 这是一个选择结构，与if类似，default表示与上面的都不匹配时运行

- 值得注意的是当你输入a，将输出优秀，但当你输入b时，会同时输出良好，差，和非法的成绩。因为没有break防止case穿透。