## 表单

### 表单标签
* form
* input
* label 说明标签，for属性值与input 的id值一致进行关联
* fieldset 表单元素编组
* legend fieldset元素的说明标签
* button
* datalist 数据列表，包含option子标签，常与input一起使用（用户可不使用option内容）
* textarea
* select ,与option一起使用，也可联合optgroup 使用

### input元素的类型
* text
* password
* button
* file
* hidden
* image
* reset
* submit
* checkbox
* date
* color
* email
* number
* month
* radio
* range
* search
* week
* url

### 表单新特性
placeholder: 输入框占位符，常用作提示用户输入的信息
autocomplete:是否保存用户输入信息，默认为on，关闭为off
autofocus:自动聚焦
required：必填项
pattern:正则验证
form: 将表单元素属性添加form属性，属性值为form表单元素的id值，表单元素可在页面任意位置（实测浏览器不支持 )
formnovalidate、novalidate:均指不验证表单，formnovalidate用于submit按钮。novalidate用于form标签

```


```
## 效果图:
![form](./form.jpg)