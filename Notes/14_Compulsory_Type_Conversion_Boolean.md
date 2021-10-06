# 强制类型转换-Boolean

将其他的数据类型转换为Boolean，使用Boolean()函数即可。

对于数字转成布尔的情况，除了0和NaN，其余都为true。

对于字符串转布尔的情况，除了空字符串，其余都为true。

**对象也会转换为true。**

Null与Undefined都转为false。

```js
var a = 123;
a = Boolean(a);
console.log(a); //true
```

## 隐式类型转换

```js
var a = 10;
a=!!a;
console.log(a); //true
console.log(typeof(a)); //boolean
```



