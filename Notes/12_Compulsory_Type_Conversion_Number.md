# 强制类型转换-Number

## 将其他数据类型转换为Number

```JS
var a = "123";
console.log(typeof(a)); //string
console.log(a); //123
```



### 方式一

*然而并没有toNumber()这种东西*

使用Number()函数将String转换为Number类型。

#### 注意事项

1. **纯数字字符串可以转成number，但是含有非数字字符时会返回NaN**
2. 空字符串以及只有空格的字符串，转换为0
3. 布尔转数字时，true转为1，false转为0
4. Null转为0
5. Undefined转为NaN



### 方式二

**对于字符串的方法**

#### parseInt() 

将一个字符串转换为一个整数，可将字符串中的有效的整数内容取出来，然后转换为Number。

```js
var a = "123px";
a = parseInt(a);
console.log(a); //123
var b = "567a123px";
b = parseInt(b);
console.log(b); //567
var c = "b567a123px";
c = parseInt(c);
console.log(c); //NaN
var d = "123.b567a123px";
d = parseInt(d);
console.log(d); //123
```

#### parseFloat()

与parseInt()类似，不同的是它可以取出有效的小数。

```js
var a = "678.123px";
a = parseFloat(a);
console.log(a); //678.123
var b = "456.678.123px";
b = parseFloat(b);
console.log(b); //456.678
```



* 对非String类型使用parseInt()或parseFloat()时，会先将其转化为String然后再取出。

```js
var a = true;
a = parseFloat(a);
console.log(a); //NaN
```

