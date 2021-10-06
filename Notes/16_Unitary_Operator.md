# 一元运算符

一元运算符，即只需要一个操作数的运算符。



* `+` 正号
  * 不会对数值产生任何影响。
* `-` 负号
  * 负号可以对数字进行符号的取反。



对于非Number值，先转成Number再进行运算。



## 隐式类型转换

可以对其他的数据类型使用`+`将其转换为number，原理和Number()函数一样。

```js
var a = true;
a = -a;
console.log(a); //-1
console.log(typeof(a)); //number

var b = "18";
b = +b;
console.log(b); //18
console.log(typeof(b)); //number
```

