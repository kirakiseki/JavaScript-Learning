# 非布尔值的与或运算

`&&`和`||`对于非布尔值的情况

对于非布尔值，进行与或运算时，会先将其转换为布尔值，然后再运算。**并且返回原值**

## 与

```js
var res = 1&&2；  //true&&true
console.log(res); //2
res = 2&&1；
console.log(res); //1
```

如果两个值都为true，则返回后面的值。


```js
var res = 0&&2；  //false&&true
console.log(res); //0
res = 2&&0；
console.log(res); //0
```

```js
var res = NaN&&0；  //false&&false
console.log(res); //NaN
res = 0&&NaN；
console.log(res); //0
```

如果两个值中有false，则返回靠前的false。



如果第一个值为true，则必然返回第二个值。

如果第一个值为false，则必然返回第一个值。

（与JS的短路系统相关）



## 或

```js
var res = 1||2;
console.log(res);  //1
res = 2||1;
console.log(res);  //2
```

如果第一个值为true，则直接返回第一个值。

```js
var res = NaN||1;
console.log(res);  //1
res = NaN||0;
console.log(res);  //0
```

如果第一个值为false，则直接返回第二个值。

