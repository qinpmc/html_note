## 文档结构

* DOCTYPE ：
1. 告诉浏览器要处理的是html文档；
2. 标记文档内容的版本
3. 浏览器根据DOCTYPE决定使用哪种渲染模式
4. 必须位于html文档第一行，不是html标签

* 渲染模式：
1. 怪异模式
2. 准标准模式
3. 标准模式
    如果网页代码不含有任何声明，那么浏览器就会采用怪异模式解析，
    如果你的网页代码含有DTD声明，浏览器就会按你所声明的标准解析

* 文档结构标签
  html、head、title、meta、link、script、body

```
<!DOCTYPE HTML>
<html>
<head>
    <title>Example</title>
    <base href="http://titan/listings/"/>
    <meta name="author" content="Adam Freeman"/>
    <meta name="description" content="A simple example"/>
    <meta charset="utf-8"/>
    <link href="theme.css" rel="stylesheet" type="text/css">
    <script src="1.js" type="text/javascript" ></script>
</head>
<body>
<p>
    I like apples and oranges.
</p>
</body>
</html>
```