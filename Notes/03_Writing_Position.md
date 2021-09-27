# JS编写位置

可以将JS代码编写到标签`onclick`属性中，点击按钮执行代码

```html
<button onclick="alert('Hello');">Click1</button>
```

也可以加到链接`href`属性上，点击超链接执行代码

```html
<a href="javascript:alert('Hello');">Click1</a>
```

当`href="javascript:;"`创建一个点击后无动作的超链接

```html
<a href="javascript:;">Click1</a>
```



**虽然JS代码可以写在标签属性中，但这种属于结构与行为的耦合，不便于后期维护，不推荐使用**



可以将JS代码编写到`<script>`标签中



可以将JS代码编写到外部的`*.js`的文件中，并使用`<script>`标签引入

```html
<script type="text/script" src="js/script.js"></script>
```

写到外部文件中可以在不同页面中复用，也可利用浏览器的缓存机制。

**但`<script>`标签一旦用于引入外部文件，就不能再其中编写代码了，即使写了，浏览器也会忽略。**



+ JS在页面中按照编写或者引入的顺序执行，即先编写或引入的更先执行。