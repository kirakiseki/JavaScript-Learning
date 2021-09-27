# Number

只有最开始声明变量时需要使用`var`，之后使用或复制同一变量时不用重新声明。

**变量仅会保留最后一次更改的值。**

# Number

在JS中包括整数，浮点数都属于`Number`类型。

```js
var a = 123;   //Number类型
var b = "123"; //String类型
```

可以使用`typeof`运算符来检查一个变量的类型。

```js
console.log(typeof(a)); //输出number
console.log(typeof(b)); //输出string
```

JS中可以表示的最大值为`Number.MAX_VALUE`，其值为1.7976931348623157e+308。

如果使用`Number`表示的数字超过了最大值，则会返回`Infinity`正无穷。同理，也会返回`-Infinity`负无穷。**实际上，`Infinity`是一个字面量。**

```js
console.log(Number.MAX_VALUE); //输出1.7976931348623157e+308
console.log(Number.MAX_VALUE*Number.MAX_VALUE); //输出Infinity
console.log(-Number.MAX_VALUE*Number.MAX_VALUE); //输出-Infinity
console.log(typeof(Infinity)); //输出number
```



`NaN`也是一个特殊的数字，表示Not a Number。**实际上，`NaN`也是一个字面量。**

```js
console.log("abc"*"bcd"); //输出NaN
console.log(typeof(NaN)); //输出number
```



JS中可以表示的最小值为`Number.MIN_VALUE`，其值为5e-324。是JS能表示的大于0的最小值（最小的正浮点数）。



在JS中，整数的运算基本可以保证精度。

```js
var c = 123 + 456;
```

但是在算浮点数的时候可能会出现问题，如著名的问题：

```js
var c = 0.1 + 0.2; //输出0.30000000000000004
```

涉及到计算机内部的数据储存以及标准的问题，这里不再展开。

故在JS中进行浮点运算时可能得到一个不精确的结果。





