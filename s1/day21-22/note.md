jQuery
# 1. 概述
## 1. 是什么？
JavaScript外部脚本（库）
## 2. 怎么用？
1. 下载 [https://jquery.com/download/](https://jquery.com/download/)
2. 链接
```
<script src="js/jquery-3.7.0.js"></script>
```
## 3. 为什么？
1. 提高开发效率（JS → jQuery）
2. JS：通过**事件响应**来控制网页中的所有**元素（增删改查）**
3. 执行效率低于原生DOM
# 2. 网页元素控制
## 1. 获得元素
### 1. 筛选器
```
$("selctor")  括号中是选择器/筛选器
document.getElementById("id") == $("#id")
```
> DOM对象  vs  jQuery对象
```
$("#id")
$(".className")
$("tagname")
$("E>F")
```
### 2. 索引器（获取index的元素）
```
jqueryObj.eq(index)  //从0开始的 -- jQuery对象
jqueryObj.get(index)  //从0开始的 -- DOM对象
jqueryObj[index] //从0开始的 -- DOM对象
```
### 3. 对象转换
dom→jQuery   $(dom)
jquery→dom   jquery[0]
## 2. 修改元素
### 1.修改文本
1. DOM : domobj.innerHTML / innerText
2. jQuery: jobj.html()/text() //括号中没有参数（读），有参数（写）
3. 扩展：jQuery筛选器得到的对象不止一个，不需要循环，自动对每一个元素进行操作
### 2.修改值
1. DOM : domobj.value 
2. jQuery: jobj.val() //括号中没有参数（读），有参数（写）
### 3.修改/得到属性
1. DOM : domobj.setAttribute("属性","值")   domobj.getAttribute("属性") 
2. jQuery: jobj.attr("属性","值")   jobj.attr("属性")
### 4.修改CSS样式
1. 修改一个样式 ：  jobj.css("属性","值")
2. 修改多个样式：   jobj.css({"属性":"值","属性":"值","属性":"值"})
3. 添加/移除定义好的class addClass/removeClass
## 3. 事件响应
1. 获得元素，然后给元素的**对应事件**绑定**处理程序**
```
document.querySelector("button").onclick = fun;
$("button").click(fun)
```
2. 事件监听，获得元素，然后给元素**添加事件监听**，添加事件名称、响应程序、是否捕获型
```
document.querySelector("button").addEventListener("click",fun,true);
document.querySelector("button").removeEventListener("click",fun,true);
```
```
事件绑定
$("button").bind("click",fun)
$("button").one("click",fun)
$("button").unbind("click")
```
3. 事件
> window.onload 页面加载  load() × ready()  √
> onload 只允许存在一次，页面内容（结构tag+内容）加载完毕
> ready 存在多次，页面结构加载完毕
> 扩展：ready简写
4. 链式编程（对象保持不变，可以一直调用该对象的方法）
## 4. 扩展知识
### 1. 单选多选属性
1. attr() 方法：页面渲染之后的节点属性
2. prop() 方法: 节点对象的属性
3. 判断是否被选用 is(":checked")
### 2. 其他筛选器
```
$("selector:first")
$("selector:last")
$("selector:eq(index)")
$("selector:lt(index)")
$("selector:gt(index)")
$("selector:odd")
$("selector:even")
$("selector:disabled")
$("selector:empty")
$("selector:checked")
$("selector:hidden")
$(":text")
$(":password")
$(":radio")
$(":checkbox")
```
# 3. 节点操作
1. 创建节点 ```$("<img/>")```
2. 添加到网页中
```
parentNode.append(temp); //追加子元素（最后一个孩子）
parentNode.preppend(temp); //追加子元素（第一个孩子）
siblingNode.after(temp); //追加在某个节点之后（兄弟）
siblingNode.before(temp); //追加在某个节点之前（兄弟）
```
3. 删除节点
```
node.remove();
```
# 4. 基于jQuery的Ajax
```
$("selector").load("URL #id"); //将URL请求得到的数据中的id片段写到selector中

$.get(url,jsondata,function(d){})
```