# 相等运算符

比较两个值是否相等。相等则返回true，否则返回false。

使用`==`来做相等运算。

```js
console.log(1==1); //true
console.log("1"==1); //true
```

当使用相等运算比较两个值时，如果值的类型不同，则会将其转换为相同的类型，然后再进行转换。

```js
console.log(true=="1"); //true
console.log(true=="hello"); //false
```

布尔值和字符串相比，都转换成Number类型。

```js
console.log(null==0); //false
```

此时并没有转换成Number



undefined衍生自null，所以这两个值进行相等判断时，会返回true。

```js
console.log(null==undefined); //true
```

NaN不和任何值相等，包括本身。

```js
console.log(NaN==NaN); //false
```



**判断b的值是不是NaN**

```js
var b = NaN;
console.log(b == NaN); //false
```

可以通过isNaN()函数来判断一个值是不是NaN。

```js
var b = NaN;
console.log(isNaN(b)); //true
```



# 不相等运算符

不相等用来判断两个值是否不相等，如果不相等返回true，否则返回false。

使用`!=`来进行不相等运算。

```js
console.log(10!=5); //true
console.log("abcd"!="abcd"); //false
console.log("1"!=1); //false
```

不相等也会对变量进行自动类型转换，如果转换后相等，也会返回false。



# 全等运算符

`===`用来判断两个值是否相等，它和相等类似，不同的是，它不会做自动类型转换。

如果两个值的类型不同，直接返回false。

```js
console.log("123"===123); //false
console.log(null === undefined); //false
```

# 不全等运算符

`!==`用来判断两个值是否不全等，和不等类似，不同的是，它不会做自动的类型转换。

如果两个值的类型不同，直接返回true。