# 关系运算符

通过关系运算符可以比较两个值之间的大小关系。

关系成立则返回true，关系不成立则返回true。

## >

判断符号左侧的值是否大于右侧的值。

```js
console.log(5>10); //false
console.log(5>4);  //true
```

## >=

判断符号左侧的值是否大于或等于右侧的值。

## <

判断符号左侧的值是否小于右侧的值。

## <=

判断符号左侧的值是否小于或等于右侧的值。



## 对于非数值的情况

```js
console.log(1>true); //false
console.log(1>=true); //true
console.log(1>"0"); //true
console.log(10>null); //true
console.log(10>"hello"); //false "hello"->NaN
console.log(true>false); //true
console.log("1"<"5"); //true
console.log("11">"5"); //false
console.log("a"<"b"); //true
console.log("abc"<"b"); //true
console.log("bbc"<"b"); //false
console.log("111212121"<"5"); //true
console.log("111212121"< +"5"); //false
```

对于非数值进行比较时，会将其转换成数字，然后再比较。

任何值和NaN做任何比较都是false

符号两侧都是字符串时，不会将其转换为数字进行比较，而是分别比较字符串中字符的Unicode编码。

比较字符编码时，是一位一位进行比较。如果两位一样，则比较下一位。可以借用它来对英文进行排序。比较中文没啥意义(

如果比较的是两个字符串型的数字，可能会得到不可预期的结果。

+ 在比较两个字符串型的数字时，一定要转型。