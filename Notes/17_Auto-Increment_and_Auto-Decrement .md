# 自增和自减

## 自增

使变量在自身的基础上增加1。

对一个变量自增以后，原变量的值会立即自增1。

运算符 `++`

自增分两种：

+ 后++(a++)
+ 前++(++a)

无论是a++还是++a；都会立即使原变量的值自增1。

a++的值等于原变量自增前的值，++a的值等于原变量自增后的值。

```js
var a = 1;
console.log(a++); //1
var b = 1;
console.log(++b); //2
```

## 自减

使变量在自身的基础上减1。

与自增类似，自建也分为前后自减两种。