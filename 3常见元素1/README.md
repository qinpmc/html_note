# 常见元素1

## a 标签
1. 属性 href target等
```
 I like <a href="http://en.wikipedia.org/wiki/Apples">apples</a> and
        <a href="http://en.wikipedia.org/wiki/Orange_(fruit)">oranges</a>.
        You can see other fruits I like <a href="#fruits">here</a>.

        <p id="fruits">
            I also like bananas, mangoes, cherries, apricots, plums, peaches and grapes.
        </p>
        如果找不到指定id元素，浏览器会查找name属性与之匹配的元素(a标签才行)
        You can see other fruits I like <a name="fruits">here</a>.
```
2. 文字标记元素
* em 强调内容，通常斜体
* i 表示与周围内容有本质区别，常用于外文词语、科技术语等,样式为斜体
* s 表示某段文字不再正确，样式为删除线
* b 并不表示特别的强调或重要性，通常会对内容加粗
* strong 表示重要的内容，样式为加粗  
* u 凸显内容，样式为下划线
