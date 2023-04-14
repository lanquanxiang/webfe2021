# 1. 函数function
1. 使用 function关键词来声明函数
2. 使用 var 来声明一个函数变量
3. 使用 new 构造一个函数对象
# 2. 常见对象 element
1. 获取网页元素 ele = document....
2. 修改/获取元素的文本  ele.innerHTML
3. 修改/获取元素的属性  ele.attr [id|value]
> ele.setAttribute("attr",value) 
> ele.getAttribute("attr")
# 3. 函数的调用
# 4. 数组
1. 数组的初始化
> ```var a = [];可以在括号中填写默认值```
> ```var b = new Array();可以在括号中填写默认值```
2. 与Java数组的区别
> 长度不固定
> 数组中可以装不同数据类型
> 不存在数组越界
3. 数组常用方法
> A.concat(B) 数组合并，不会影响AB的值
> A.reverse() 倒置数组，影响A
> A.join("字符") 使用指定的字符链接所有的元素，数组→字符串 toString() ==a.join(",")
> A.unshift("任意数据") 向头部插入，返回新数组的长度
> A.shift()  删除头部元素，返回被删除的元素
> A.push("任意数据") 向尾部插入，返回新数组的长度
> A.pop() 删除尾部元素，返回被删除的元素
# 5. 字符串
1. 初始化
> var a = ""; 
> var b = new String("");
2. 常用方法
> indexOf("字符")
> substr(start,length)
> substring([start,end))
> split("字符") 与join相反，字符串→数组