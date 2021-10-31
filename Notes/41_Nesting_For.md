# 嵌套的for循环

## 正三角

通过程序，在页面中输出如下图形

```
*
**
***
****
*****
```



向`body`中输出内容

```js
document.write("test");
```



换行标签`<br />`



输出一个高为10的矩形

```js
for(var i=0;i<10;i++){
    document.write("*****<br />");
}
```





最终代码

```js
for(var i=0;i<5;i++){
    for(var j=0;j<i+1;j++){
        document.write("*");
    }
    document.write("<br />");
}
```

内层循环控制图形某一层的宽度

外层循环控制图形的高度



## 倒三角

```
*****
****
***
**
*
```



```js
for(var i=0;i<5;i++){
    for(var j=5-i;j>0;j--){
        document.write("*");
    }
    document.write("<br />");
}
```

内层循环控制图形某一层的宽度





## 乘法表

```js
for(var i=1;i<=9;i++){
    for(var j=1;j<=i;j++){
        document.write(j + "*" + i + "=" + i*j +"&nbsp;");
    }
    document.write("<br />");
}
```

### 解决强迫症

```js
for(var i=1;i<=9;i++){
    for(var j=1;j<=i;j++){
        document.write("<span>" + j + "*" + i + "=" + i*j +"</span>");
    }
    document.write("<br />");
}
```

```css
span{
    display: inline;
    width: 50px;
}
```





