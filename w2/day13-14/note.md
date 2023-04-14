# 1. 网页元素node/element
* Live Node = document.getElementById("id")
* Live Node List = document.getElementsByClassName("class")
* Live Node List = document.getElementsByName("name")
* Live Node List = document.getElementsByTagName("tagname")
* Static Node = document.querySelector("selector")
* Static Node List = document.querySelectorAll("selector")
# 2. 获取修改元素的值/文本
1. 修改元素的值 ele.value   ele.value="新的值"
2. 修改元素的文本 ele.innerHTML/innerText   ele.innerHTML ="新的值"
# 3. 修改/获取元素的属性
1. setAttribute("name",value)
2. getAttribute("name")
# 4. 数组
## 1. 数组的初始化
> ```var a=[];```
> ```var b = new Array(); //开括号中可以填写默认值，多个值用','隔开```
## 2. 区别
> 不需要设置长度
> 不存在数组越界（1.读 undefined 2.写 中间为赋值的元素都是undefined）
> 数组中可以保存不相同的元素
## 3. 常用方法
> A.concat(B) 将A和B数组进行连接，返回连接结果，不影响AB的值
> A.shift() 将A的第一个元素删除，并返回删除的元素
> A.unshift(任意值) 将任意值视为一个元素插入到数组的头部，返回新数组的长度
> A.pop() 将A的最后一个元素删除，并返回删除的元素
> A.push(任意值) 将任意值视为一个元素插入到数组的尾部，返回新数组的长度
> A.reverse()倒置数组元素，影响A
> A.join("任意字符") 使用指定的字符连接所有元素，数组→字符串
> A.toString() == a.join(",")
# 5. Math
1. 常用方法
> Math.floor(X) 向下取整
> Math.round(x) 四舍五入
> Math.ceil(X) 向上取整
> Math.random() [0-1)之间的随机数