# break和continue

break可以用来退出switch和循环语句。

但break和continue不能用在if标签中。

break关键字，会立即终止离它最近的循环语句。

 



可以为循环语句创建一个label，来表示当前的循环。

```
label:循环语句
```

使用语句时，可以在break后跟着一个label，这样break后会结束指定的循环，而不是最近的。



continue关键字可以用来跳过当次循环。

同样，continue关键字也是默认只对最近的循环起作用。

continue也可以使用label方法控制循环的执行。



## 计时器

```js
console.time("test");
```

开启一个名字为test的计时器

```js
console.timeEnd("test");
```

停止一个名字为test的计时器

