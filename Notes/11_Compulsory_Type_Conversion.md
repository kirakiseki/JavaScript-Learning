# 强制类型转换

将一个数据类型强制转换为其他的数据类型。

类型转换主要指将其他的数据类型转换为String，Number，Boolean。

## 转换为String

```JS
var a = 123;
console.log(typeof(a)); //number
console.log(a); //123
```

### 方法1

调用被转换数据类型的`toString()`方法。

该方法不会影响原变量，而是返回转换后的结果。

如调用a的`toString()`的方法：

```js
var b = a.toString();
console.log(typeof(b)); //string
console.log(b); //123
```

或者直接将a转换为string：

```js
a=a.toString();
```

#### 局限性

null和undefined两个类型没有toString()方法，调用后会报错。

### 方法2

调用`String()`函数，并将被转换的数据作为参数传递给函数。

函数同样具有返回值。

```js
a = String(a);
```

```js
var a = null;
a = String(a);
console.log(typeof(a)); //string
console.log(a); //null
```

**使用String()函数时，对于Number和Boolean实际上就是调用toString()方法，对于Null和Undefined，不会调用toString()方法，而是直接转换为"null"和"undefined"**

