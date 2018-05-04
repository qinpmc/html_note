## DOCTYPE   
1.告诉浏览器要处理的是html文档;  
2.标记文档内容的版本;  
3.浏览器根据DOCTYPE决定使用哪种渲染模式;  
  
## 渲染模式    
1.怪异模式  
2.准标准模式  
3.标准模式  
  如果网页代码不含有任何声明，那么浏览器就会采用怪异模式解析，   
  如果你的网页代码含有DTD声明，浏览器就会按你所声明的标准解析

## 文档结构元素
 + html、head、body

## 元数据元素
1.元数据元素位于head标签中
2.主要包括：
  * title
  * base ,局部属性 href（可写绝对和相对路径） targt
  * meta ，说明文档

## 元数据元素 meta
1. 示例
```
<!DOCTYPE HTML>
<html>
    <head>
        <title>Example</title>
        <base href="http://titan/listings/"/>
        <meta name="author" content="Adam Freeman"/>
        <meta name="description" content="A simple example"/>
        <meta charset="utf-8"/>
    </head>
    <body>
        <p>
            I like <code id="applecode">apples</code> and oranges.
        </p>
        <a href="http://apress.com">Visit Apress.com</a>
        <a href="page2.html">Page 2</a>
    </body>
</html>
```
