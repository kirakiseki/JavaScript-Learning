# 逻辑运算符

三种逻辑运算符，用来进行逻辑判断

| 运算符 | 操作 |
| ------ | ---- |
| !      | 非   |
| &&     | 与   |
| \|\|   | 或   |

## 非

`！`可以对一个值进行非运算。

```js
var a = true;
a=!a;
console.log(a); //false
```

非运算即对一个布尔值进行取反操作。

true->false

false->true



对一个值进行两次取反，它的值不会变化。

对非布尔值进行运算，会先转化成布尔值，然后再进行运算。

```js
var b = 10；
b=!b;
console.log(b); //false
console.log(typeof(b)); //boolean
```

可以利用该特点进行**隐式类型转换**，原理和Boolean()函数一样。

```js
var c = 10;
c=!!c;
console.log(c); //true
console.log(typeof(c)); //boolean
```

## 与

`&&`可以对符号两侧的值进行与运算，并返回结果。真值表如下。

| A    | B    | A&&B |
| ---- | ---- | ---- |
| 1    | 1    | 1    |
| 1    | 0    | 0    |
| 0    | 1    | 0    |
| 0    | 0    | 0    |

只有两个值同时为true，才返回true；只要有一个值为false，就返回false。

JS中的与属于短路的与。即如果第一个值为false，不会再看第二个值。

```js
true&&console.log("test1"); //test1
false&&console.log("test2"); //不会输出
```

## 或

`||`可以对符号两侧的值进行或运算，并返回结果。真值表如下。


| A    | B    | A\|\|B |
| ---- | ---- | ------ |
| 1    | 1    | 1      |
| 1    | 0    | 1      |
| 0    | 1    | 1      |
| 0    | 0    | 0      |

即两侧只要有一个为true，结果即为true。

JS中的或同样也是短路的或，即如果第一个值为true，不会再检查第二个值。

```js
true||console.log("test1"); //不会输出
false||console.log("test2"); //test2
```

