# 1. 自定义对象
1. 空白对象 var obj = {};
2. 有属性对象 var obj = json {属性:属性值{},属性:属性值} 
3. 属性值：基础数据类型、数组、对象、函数
4. 读取属性的方法 obj.attr  obj["attr"]
5. 如果读取了不存在的属性，属性值为undefined
# 2. 常用对象
## 1. 数组
1. 初始化
> var a1 = [];
> var a2 = new Array();
2. 常用方法
> a.concat(b) 数组连接，返回新数组(a,b不发生改变)
> a.shift() 删除数组的第一个元素，返回的是第一个元素（a会发生改变）
> a.unshift(s) 将s这个元素插入到数组的最前面，返回新数组的长度
> a.push(s)将s这个元素插入到数组的最后面，返回新数组的长度
> a.pop() 删除数组的最后元素，返回的是最后一个元素（a会发生改变）
> a.reverse() 倒置数组，返回新的数组
> a.join("字符") 使用指定的字符来连接数据的所有元素，返回一个字符串 数组→字符串
3. 扩展方法
> Live Node = document.getElementById("id")
> node.attr = ""  或 node.setAttribute("attr","新的值")
> node.getAttribute("attr")
> node.innerHTML = "新的文本" 或  node.innerHTML
## 2. 字符串string
1. 初始化
> var s = "";
> var s = new String("");
2. 常用方法
> indexOf/charAt
> substr/substring
> split  字符串→数组
