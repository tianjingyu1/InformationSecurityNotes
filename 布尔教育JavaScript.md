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
4. substr(num1,[num2])截取字符串
5. toLowerCase() 转换成小写
6. toUpperCase() 转换成大写
7. replace(str1,str2) 字符串替换

Date日期对象
1. getYear() 返回年份(2位或4位)
2. getFullYear() 返回年份(4位)
3. getMonth() 返回月份 0-11
4. getDate() 返回日期1-31
5. getDay() 返回星期数0-6
6. getHouse() 返回小时数0-23
7. getMinute() 返回分钟数0-59
8. getSeconds() 返回秒数0-59
9. getMilliseconds() 返回毫秒数0-999

Math数学对象
1. cell(数值) 大于或等于该数的最小整数
2. floor(数值) 小于或等于该数的最大整数
3. min(数值1，数值2)返回最小值
4. max(数值1，数值2)返回最大值
5. pow(数值1，数值2)返回数值1的数值2次方
6. random() 返回随机数0-1
7. round(数值) 四舍五入
8. sqrt(数值) 开平方根

数组对象
1. concat() 返回一个由两个数组合并组成的新数组
2. join() 返回一个由数组中的所有元素连接在一起的String对象
3. pop() 删除数组中的最后一个元素并返回该值
4. push() 向数组中添加新元素，返回数组的新长度
5. shift() 删除数组的第一个元素并返回该值
6. unshift() 返回一个数组，在该数组的头部插入了指定的元素
7. sort() 返回一个元素被排序了的Array对象
8. reverse() 返回一个元素反序的Array对象
9. slice() 返回数组的一个片段
10. splice() 从数组中删除元素

# window对象

window对象是浏览器宿主对象和JS语言无关

方法：
window.alert(message)
window.confirm(message)
window.prompt(message[, default])
window.close() 关闭窗口
window.print() 打印

window.serIntval(表达式，毫秒);
window.ckearIntval(定时器对象);
window.setTimeout(定时器对象);

子对象
navigator location history screen document

# var的重要性

作用域

# 找对象

1. 按id找 返回的是对象
2. 按标签找 div,p,input,...  返回的是对象的集合
3. 对于表单元素，可以按name来查询 返回的是对象集合
4. 按类名找  返回的是对象集合
5. 找子对象children,parent  非标准，但兼容很好，不包括空白节点（子节点 父节点）

# 操作对象的属性

普通属性可以通过对象.标签属性 来访问
CSS属性通过对象.style属性

标签属性与DOM对象属性的对应关系，绝大部分二者是相同的
也有例外，如class属性

css属性与DPM对象属性的想对应关系，二者通过obj.style.css属性名相对应
如css属性带有横线，如border-top-style，则把横线去除并横线后的字母大写

# 获取对象在内存中计算的样式

对于<style></style>中的css属性值可以用obj.currentStylr和window.getComputedStyle()来获取
获取的对象是只读的，要改样式还得靠obj.style

# 删除对象

1. 找到对象
2. 找i到他们的父对象parentObj
3. parentObj.removeChild(子对象)

# 联动菜单 
# 定时器 window.setTimeout() 循环调用

# 清除定时器 clearlnterval() clearTimeout()

事件对象包含事件相关的信息，如鼠标，时间，触发的DOM对象等
事件对象被系统传递给事件函数的第1个参数
事件对象的属性在IE/w3c略有不同
一个重要的事件属性：target, srcElement(),代表事件发生的所在DOM对象

事件委托

# 正则表达式
patt.test() 检测是否符合