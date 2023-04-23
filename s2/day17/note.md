# 1. 对节点（node、element）的操作（document）
## 1. 获得元素
Live Node = document.getElementById("id")
Live Node List = document.getElementsByClassName("class")
Live Node List = document.getElementsByName("name")
Live Node List = document.getElementsByTagName("tagname")
Static Node = document.querySelector("selector")
Static Node List = document.querySelectorAll("selector")
## 2. 修改元素
> 修改属性 setAttribute()/获得getAttribute()
> 修改文本 innerHTML/innerText
## 3. 增加节点
> parentNode
> firstChild
> lastChild
> childNodes
1. 增加节点流程
> 创建节点 createElement("a")
> 为节点增加必要的内容(属性、文本)
> 将节点添加到网页中 parentNode.appendChild()
> ele.parentNode.insertBefore(newEle,ele);
2. 批量增加（刷新DOM一次）
> 创建文档碎片
> 创建n个节点，将节点加入文档碎片
> 文档碎片加入网页中
## 4. 删除节点
```
ele.parentNode.removeChild(ele);
```
# 2. 对BOM的操作（window）
## 1. 属性(掌握)
```
window.location.href //当前的URL地址（读、写）
```
## 2. 打开和关闭窗口（了解）
```
	var w = window.open("URL")
	w.close();
```
## 3. 交互框（重点）
1. 警告框
```alert("警告内容!")```
2. 确认框
```
	var res = confirm("确认内容?")  //true/false
```
3. 询问框
```
	var str = prompt("问题","默认答案");
```
## 4. 计时器
1. 只执行一次
```
	var t = setTimeOut(函数名,mills-time);
	clearTimeOut(t);
```
2. 周期性执行
 ```
	var t = setInterval(函数名,mills-time);
	clearInterval(t);
```
3. JS执行机制（面试）
> 计时器中的代码为异步执行
## 5. 其他
> 窗口的历史记录window.history
> 将信息保存cookie：document.cookie