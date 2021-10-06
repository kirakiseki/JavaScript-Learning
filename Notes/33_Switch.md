# 条件分支语句

条件分支语句也叫switch语句

```js
switch(条件表达式){
    case 表达式1:{
        语句1
        break;
    }
    case 表达式2:{
        语句2
        break;
    }
    case 表达式3:{
        语句3
        break;
    }
    default:{
        语句4
        break;
    }
}
```



## switch...case...语句

在执行时会依次将case后的表达式和switch后的条件表达式的值进行**全等**比较，

如果比较结果为true，则从当前case处开始执行代码；

**可以在case后加break关键字，这样可以确保只执行当前case中的代码，而不会执行其他的case。**

如果比较结果为false，则继续进行比较。

如果所有的比较结果都为false，则执行default中的语句。



switch与if语句的功能实际上是有重复的，使用if可以实现switch的功能，使用switch也可以是实现if的功能。实现过程中可以根据自己的习惯选择。