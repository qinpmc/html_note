# html_总结

## html元素分类
### 行内元素
   span、a 、input、button、select、textarea、label、small、strong、em、i、mark、s、b、sup、sub、u、script
   1. 不独占一行
   2. 排列方式：从左到右
   3. 设置宽高不起作用，如果要起作用，可将其转换为 块/行内块，display:block/display:inline-block
   4. 不设置宽高是它本身内容的宽高
   5. 自带display:inline
   6. 行内元素里不能嵌套块元素（a标签除外），a标签不能嵌套a标签，浏览器总是解析成并列的a


### 块元素
    div、p、h1-h6、ul、ol、li、dl、dt、dd、table、hr、form、figure、figcaption、
    article、aside、nav、menu、canvas、header、main、section、footer
    
    
    
   1. 独占一行
   2. 排列方式：从上到下
   3. 可以设置宽高以及盒模型的其他属性
   4. 不设置宽高的情况下，它的宽度是父元素的宽度，高度是本身内容的高度
   5. 自带display:block
   6. 块元素可嵌套行内元素，ul，ol中只能是li；dl中只能是dt和dd；p标签中不能嵌套块元素(被浏览器分割为多个p)，包括p自身，但可以嵌套行内元素


### 行内块元素
    img 
    1. 自带display:inline-block

### 标签语义化
    1. 合适的标签做合适的事情，如段落用p标签，标题用h1~h6
    2. 标签语义化为浏览器和搜索引擎服务
    3. 使用标签语义化的原因：
     - 利于SEO优化
     - 样式丢失时，也可以较好的呈现结构
     - 更好地支持各种终端，如无障碍阅读和有声小说等
     - 利于团队开发和维护，遵循W3C标准，有利于减小代码差异，提高开发和维护的效率



### 长度值
1. px
2. em：本元素给定字体的 font-size 值，如果元素的 font-size 为 14px ，那么 1em = 14px；如果 font-size 为 18px，那么 1em = 18px
3. 百分比  p{font-size:12px;line-height:130%} line-height = 15.6px


### 颜色值
1. 名称: p{color:red;}
2. RGB颜色
由 R(red)、G(green)、B(blue) 三种颜色的比例来配色：p{color:rgb(133,45,200);}
或者p{color:rgb(20%,33%,25%);}

3. 十六进制颜色

每一项的值由 0-255 变成了十六进制 00-ff: p{color:#00ffff;},可省略为p{color:#0ff;}