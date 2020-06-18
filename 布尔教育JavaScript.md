# JS和DOM

浏览器有渲染html的功能，把html源码再内存里形成一个DOM对象，就是文档对象
我们在html里写一个js代码，js代码被引擎所执行，而执行的结果，就是对DOM的操作

浏览器是宿主，但js的宿主不限于浏览器，也可能是服务器端，如比较流行的服务器端框架Node.js

# JS引入

script标签写在head和body位置
多段script的执行顺序
按引入顺序，逐段执行

# 变量声明

JS的变量名可以用_、数字、字母、$,组成，且数字不能开头
声明变量用var变量名来声明
js的变量名，区分大小写
不用var，会污染全局变量

# JS变量类型

数值类型 字符串类型 布尔类型 null类型 undefined型

undefined 代表没有原生数据
null 代表没有对象

# JS运算符

特殊：拼接运算符 "+"
一旦碰到非法数字，后面的运算理解为拼接
逻辑运算，返回的是最早能判断表达式结果的那个值（短路）

# 控制结构

# 对象操作

length substr join split

String字符串对象
1. length属性：长度
2. concat(String) 连接两个或更多个字符串
3. indexOf(String) 返回出现字符串的位置
4. 