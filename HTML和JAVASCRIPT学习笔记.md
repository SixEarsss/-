# HTML和JAVASCRIPT学习笔记

1. **HTML** 定义了网页的内容
2. **CSS** 描述了网页的布局
3. **JavaScript** 控制了网页的行为

### 1.什么是 HTML?

HTML 是用来描述网页的一种语言。

- HTML 指的是超文本标记语言:**H**yper**T**ext**M**arkup**L**anguage
- HTML 不是一种编程语言，而是一种**标记**语言
- 标记语言是一套**标记标签**(markup tag)
- HTML 使用标记标签来**描述**网页
- HTML 文档包含了HTML**标签**及**文本**内容
- HTML文档也叫做web页面

### 2.简单示例：

![img](https://www.runoob.com/wp-content/uploads/2013/06/02A7DD95-22B4-4FB9-B994-DDB5393F7F03.jpg)

- **<!DOCTYPE html>**声明为 HTML5 文档
- **<html>**元素是 HTML 页面的根元素
- **<head>**元素包含了文档的元（meta）数据，如**<meta charset="utf-8">**定义网页编码格式为**utf-8**。
- **<title>**元素描述了文档的标题
- **<body>**元素包含了可见的页面内容
- **<h1>**元素定义一个大标题
- **<p>**元素定义一个段落

### 3.什么是JAVASCRIPT：

JavaScript 是脚本语言

JavaScript 是一种轻量级的编程语言。

JavaScript 是可插入 HTML 页面的编程代码。

JavaScript 插入 HTML 页面后，可由所有的现代浏览器执行。

### 4.JavaScript的一些重要用法：

##### JavaScript：直接写入 HTML 输出流

##### 实例

```
document.write("<h1>这是一个标题</h1>"); document.write("<p>这是一个段落。</p>");
```



| ![lamp](https://www.runoob.com/images/lamp.jpg) | 您只能在 HTML 输出中使用 document.write。如果您在文档加载后使用该方法，会覆盖整个文档。 |
| ----------------------------------------------- | ------------------------------------------------------------ |
|                                                 |                                                              |

------

##### JavaScript：对事件的反应

##### 实例

alert() 函数在 JavaScript 中并不常用，但它对于代码测试非常方便。

------

##### JavaScript：改变 HTML 内容

使用 JavaScript 来处理 HTML 内容是非常强大的功能。

##### 实例

```
x=document.getElementById("demo");  //查找元素 x.innerHTML="Hello JavaScript";    //改变内容
```



------

##### JavaScript：改变 HTML 图像

本例会动态地改变 HTML <image> 的来源（src）：

##### 点亮灯泡

<script> function changeImage() {     element=document.getElementById('myimage')     if (element.src.match("bulbon"))     {         element.src="/images/pic_bulboff.gif";     }     else     {         element.src="/images/pic_bulbon.gif";     } } </script> <img id="myimage" onclick="changeImage()" src="/images/pic_bulboff.gif" width="100" height="180">

点击以下灯泡查看效果：

![img](https://www.runoob.com/images/pic_bulboff.gif)

点击灯泡就可以打开或关闭这盏灯

> 以上实例中代码 **element.src.match("bulbon")** 的作用意思是：检索 **<img id="myimage" onclick="changeImage()" src="/images/pic_bulboff.gif" width="100" height="180">** 里面 src 属性的值有没有包含 **bulbon** 这个字符串，如果存在字符串 **bulbon**，图片 **src** 更新为 **bulboff.gif**，若匹配不到 **bulbon** 字符串，**src** 则更新为 **bulbon.gif**

JavaScript 能够改变任意 HTML 元素的大多数属性，而不仅仅是图片。

------

##### JavaScript：改变 HTML 样式

改变 HTML 元素的样式，属于改变 HTML 属性的变种。

##### 实例

```
x=document.getElementById("demo")  //找到元素  x.style.color="#ff0000";           //改变样式
```



------

##### JavaScript：验证输入

JavaScript 常用于验证用户的输入。

##### 实例

```
if isNaN(x) {    alert("不是数字"); }
```

