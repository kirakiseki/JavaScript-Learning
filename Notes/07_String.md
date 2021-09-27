# 字符串

数据类型就是指字面量的类型。

在JS中共有六种数据类型，如下表

| 数据类型  | 名称   | 示例    |
| --------- | ------ | ------- |
| String    | 字符串 | "hello" |
| Number    | 数值   | 123     |
| Boolean   | 布尔值 | true    |
| Null      | 空值   |         |
| Undefined | 未定义 |         |
| Object    | 对象   |         |

String Number Boolean Null Undefined 属于`基本数据类型`

Object 属于`引用数据类型`



# 字符串

在JS中使用字符串需要使用引号引起来，双引号或者单引号均可，但不能混用，应当成对使用。

**引号不能嵌套**

双引号里不能放双引号，单引号里不能放单引号。但是交错使用是可以的。

在字符串中可以使用`\`作为转义字符，在表示一些特殊符号时可用来进行转义。

（Q: 多层嵌套怎么办呢?）

```js
var str1 = "hello";
var str2 = 'I say "Hey Hey Hey START:DASH".';
var str2 = 'I say \"Hey Hey Hey START:DASH\".';
```

 

### 常见的转义

`\n`  换行

` \t ` 制表符 

`\" ` "

`\'`  '

`\\`  \



```javascript
alert("str"); //输出字面量"str"
alert(str)    //输出变量str
```

