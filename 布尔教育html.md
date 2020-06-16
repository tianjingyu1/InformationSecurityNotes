# 什么是html文档？

HTML指的是超文本标记语言（Hyper Text Markup Language）

1. html是文档的一种(.html,.pdf,.doc,.红头文件)

任何工具都可以编写

<DOCTYPE ...>文档类型
strict.dtd 严格的 transitional.dtd 兼容的 frameset.dtd 松散的

从上到下布局

用div布局，css控制

浮动布局

清除浮动


常犯错误：
1. 不加doctype 导致低版本IE，解析效果不一样
2. id为数字
3. 文件编码与charset申明不一致

盒模型：

盒子的border 3要素 宽，形状，颜色

一个盒子，有margin，border,padding，实占多少空间？
竖直方向：height + padding-top + padding-bottom + border-top + border-bottom + margin-top +margin-bottom
水平方向：width + padding-left + padding +right + border-left + border-right + margin-left + margin-right

- 块级元素 能独占一行 能设宽高 竖直方向的margin-padding有，可以设置
- 内联元素 不能独占一行 不能设宽高 竖直方向的margin-padding没有，也不可以设置
内联元素又被称为行内元素

内联与块状转化
display:block/inline

段落缩进：text-indent

text-align:文本方向

文本装饰线：text-decoration

letter-spacing 文本字体间距

color：颜色

font-style：字体样式

font-weight：字体重量（加厚）

font-size：字体大小

line-height：行高

font-family：字体

你设置的字体，客户机器上未必有

sans-serif 

serif

background-color：背景颜色

background-image：背景图片

background-repeat：背景图片是否重复

background-attachment：背景图片是否固定

background-position：图片位置

选择器：id选择器，class选择器，标签选择器，派生选择器

### 控制越精细优先级越高

css四种引用方式：
1. 外部链接一个CSS文件，我们在HTML头部分标明：<link href="css/my.css" rel="stylesheet" type="text/css"/>
2. 头部直接写入CSS：<style type="text/css">div{margin:0;padding:0;border:1px solid red;}</style>
3. 外接多个CSS文件时：<style type="text/css">$import url(my.css);</style>
4. 直接在html标签里写入对这个标签的CSS控制，如：<div style="border:1px solid red;">测试信息</div>
（页内style标签 外部css文件 行内style标签 import导入）

相同的元素，如li，在不同的浏览器下，显示的效果稍有不同
是因为，浏览器对各元素的margin,border,font-size等略有不同，
如果杜绝这种情况，我们通过css强制让所有元素的属性值都一样
这个过程，叫做css初始化

## html标签
### 无语义标签

div 块级元素，布局分块用
span 内联元素，选择文字用

### 有语义标签

h1-h6 标题
p 段落
img 图片
embed 视频
a 超链接和锚点
ul 无序列表
ol 有序列表
table 表格

### h p

h1~h6系列 表示1-6号标题，字越来越小
p表示段落，在新闻网站中，h和p经常一起出现，新闻标题一般用h表示，而新闻的每一段内容，适合用p标签

### img

img src代表资源 alt代表注释，用于网页分析 title表示标题，鼠标放上去显示

img是内联元素，同时是内联替换元素，替换元素是能设置宽高的

### a

超链接 href表示链接地址 target表示打开链接方式 title鼠标放上去显示

a标签为内联元素

### 锚点

使用a标签做锚点

在输入框中输入#p2即可转到该锚点

### 伪类

css允许我们针对a标签的4中状态设置各自的css特性，叫做css伪类

hover 鼠标放上去

active 点击瞬间

link 普通状态

visited 访问过的

1. active状态一般不必写
2. 一定注意，顺序是LVHA
3. a:link可以简写为a

### 字符实体

在html中，有一些字符，不适于直接写出，如&gt;&lt;

一般格式：&amp; + 实体名 + ；

常用：
&gt; &lt; &quot; &yen; &copy;

