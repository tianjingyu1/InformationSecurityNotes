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