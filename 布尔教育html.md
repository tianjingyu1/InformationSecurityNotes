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