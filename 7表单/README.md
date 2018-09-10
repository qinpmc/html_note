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

```
  <fieldset>
    <legend>健康信息</legend>
    身高：<input type="text" />
    体重：<input type="text" />
  </fieldset>
```


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



### 表单注意事项：

form表单

![](formtag.png)

get与post区别：
1. get请求提交的数据直接在地址栏可见，而post请求提交的数据在请求体中，地址栏上不可见；
2. get请求提交的数据由于在地址栏直接可见，因此不安全，而post请求提交的数据地址栏不可见，因此相对更安全；
3. get请求提交的数据的一般较小（如果太大，浏览器会截断信息，造成数据丢失），而post请求传递的参数理论上没有限制，可以很大（但实际上受限服务器的处理能力，不可能无限大）

- input name值：
name 值作为提交数据的 key值，如果没有name，浏览器提交时会忽略该input输入的值。
radio/ checkbox ,name值必须相同，代表是一组；

- label标签
label标签主要作为标识使用，比如 类型为text、password的inut输入框，前面添加label，可标识该输入框需要用户输入什么信息。
此外，label标签 for属性，其属性值取 input 输入框的id值，可以使得用户在点击label标签时，选中该input输入框，方便用户使用。


- http  get请求的长度限制

> http  get请求的长度限制取决于服务器和使用的客户端（如果有用代理，还取决于服务器或客户端使用的代理）。   
> 大多数Web服务器的限制为8192字节（8KB），这个限制通常可在服务器配置中的某处进行配置。对于客户端，HTTP 1.1规范甚至警告过这一点，   
> 以下第3.2.1章的摘录：

>    “注意：服务器应该谨慎依赖长度超过255个字节的URI，因为某些较旧的客户端或代理实现可能无法正确支持这些长度”。   

> MSIE 和Safari 浏览器的大小限制大约2KB，Opera的大小限制大约为4KB，Firefox大小限制大约8KB。因此，我们可以认为8KB是最大可能长度，    
> 并且2KB是服务器端依赖的更可接受的长度，再考虑到整个URL的长度限制，255字节是最安全的长度。  
> 如果超出浏览器或服务器中的限制，大多数服务器或浏览器将仅截断限制之外的字符而不发出任何警告。但是，某些服务器可能会发送HTTP 414错误。   
> 如果您需要发送大数据，那么最好使用POST而不是GET。它的长度限制要高得多，但更多地依赖于使用的服务器而不是客户端。  
> 通常，web服务器一般大小限制高达2GB左右，当然这也可以在服务器设置中的某处进行配置。当超过POST限制时，服务器一般将显示特定的服务器错误或异常，   
> 通常为HTTP 500错误。

### file

```
<input type="file" accept="image/gif,image/jpeg"/>
可限制上传的图片格式为gif和jpeg
```


