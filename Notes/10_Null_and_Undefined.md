# Null and Undefined

`Null`类型的值只有一个，就是null。

**null这个值专门用来表示一个空的对象。**

```js
var a = null;
console.log(typeof(a)); //输出object
```



`Undefined`类型的值也只有一个，就是undefined。

当声明一个变量，但并不为变量赋值时，它的值就为undefined。

**未声明的变量不等于未赋值的变量**

```js
var b;
console.log(typeof(b)); //输出undefined
```



