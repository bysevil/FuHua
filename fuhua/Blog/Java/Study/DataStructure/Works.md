## 1.分别计算1-100之间所有奇数和偶数的和

```java
public class four {
    public static void main(String[] args) {
        int i1=0;
        int i2=0;
        for (int i = 0; i <=100; i++) {
            if(i%2==1){
                i1=i1+i;
            }else{
                i2=i2+i;
            }
        }
        System.out.println(i1);
        System.out.println(i2);
    }
}
```

输出效果：

```java
2500
2550
```



## 2.输出所有1-1000之间能被5整除的数，且每行输出5个

```java
public class Three {
    public static void main(String[] args) {
        for(int i =1;i<=100;i++){
            if(i%5==0){
                System.out.print(i+"\t");
            }
            if(i%25==0){
                System.out.println("");
            }
        }
    }
}
```

输出效果：

```java
5	10	15	20	25	
30	35	40	45	50	
55	60	65	70	75	
80	85	90	95	100	
```

## 3.打印九九乘法表

```java
public class Two {
    public static void main(String[] args) {
        for (int i = 1; i < 10; i++) {
            for (int j = 1; j <i+1; j++) {
                System.out.print(j+"*"+i+"="+(i*j)+"\t");
            }
            System.out.println("");
        }
    }
}
```

输出效果：

```java
1*1=1	
1*2=2	2*2=4	
1*3=3	2*3=6	3*3=9	
1*4=4	2*4=8	3*4=12	4*4=16	
1*5=5	2*5=10	3*5=15	4*5=20	5*5=25	
1*6=6	2*6=12	3*6=18	4*6=24	5*6=30	6*6=36	
1*7=7	2*7=14	3*7=21	4*7=28	5*7=35	6*7=42	7*7=49	
1*8=8	2*8=16	3*8=24	4*8=32	5*8=40	6*8=48	7*8=56	8*8=64	
1*9=9	2*9=18	3*9=27	4*9=36	5*9=45	6*9=54	7*9=63	8*9=72	9*9=81	
```

## 4.输出三角形

```java
public class One {
    public static void main(String[] args) {
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

输出效果

```java
     *     
    ***    
   *****   
  *******  
 ********* 
***********
```

