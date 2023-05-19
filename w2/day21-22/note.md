jQuery
# 1. 概述
## 1. 是什么？
JavaScript的脚本库（外部脚本 *.js）
## 2. 为什么？
优化JavaScript操作（事件响应控制网页元素），提高开发效率
## 3. 怎么用？
1. 下载[https://jquery.com/download/](https://jquery.com/download/)
2. 在网页中链接该脚本
# 2. 获得网页元素
1. 筛选器
```
$("selector") //css选择器(标签、id、class、组合) 、过滤选择器
document.querySelectorAll("selector")
```
注意：如果不使用索引器，对数组中的每一个都进行操作
扩展：DOM对象(d) jQuery对象(j)
> j = $(d)
> d= j[0]
jQuery效率低于DOM
2. 索引器（获取数组中的某一个）
```
eq(index) //jQuery对象
get(index) //DOM对象
[index]
```
# 3. 修改文本
* DOM: obj.innerHTML/innerText
* jQuery: jobj.html()/text()
# 4. 修改值
* DOM: obj.value
* jQuery: jobj.val()
# 5. 修改/得到属性
* DOM: obj.setAttribute("属性","值") obj.getAttribute("属性")
* jQuery: jobj.attr("属性","值") jobj.attr("属性")
## 扩展知识
1. attribute（节点）和property（对象）的区别
2. 如果需要设置动态的属性，使用propert
# 6. 修改CSS样式
* 一个样式： jobj.css("属性","值") 
* 多个样式： jobj.css({"属性":"值","属性":"值"})
* 多个样式：
	* 定义一个class样式
	* jobj.addClass("class名字")
	* jobj.removeClass("class名字")
# 7. 其他的过滤器和筛选器[了解]
```
$("selector:first")
$("selector:last")
$("selector:odd")
$("selector:even")
$("selector:eq(index)")
$("selector:lt(index)")
$("selector:gt(index)")
$("selector:empty")
$("selector:checked")
$("selector:selected")
$("selector:disabled")
$("selector:from的type")
```
# 8. 事件
## 1. 为指定的事件附加函数
DOM:为元素的对应事件绑定函数(灵活的获取任意元素，将HTML与JS分离)
```
1. 得到元素
2. 为元素的对应事件绑定函数
<button>按钮</button>
document.querySelector("button").onclick = fun;
```
jQery：为元素的对应事件附加函数
```
1. 得到元素
2. 为元素的对应事件附加函数
<button>按钮</button>
$("button").click(fun);
```
### 扩展知识：onload VS load （×） ready（√）
> onload 页面内容（结构+资源）加载完毕之后触发，只允许存在一个
> ready 页面结构加载完毕之后触发，多次使用
## 2. 为元素添加事件监听
1. DOM（自定义事件模型、可以取消监听）
```
<button>按钮</button>
document.querySelector("button").addEventListener("click",fun,true);
document.querySelector("button").removeEventListener("click",fun,true);

```
2. jQuery 为元素绑定事件
```
<button>按钮</button>
$("button").bind("click",fun);
$("button").unbind("click");
$("button").one("click",fun);

```
# 9. 节点的创建和删除
1. 创建节点
```
var temp = $("<div></div>");
```
2. 追加节点
```
parentNode.append(childNode); //追加子节点（最后一个）
parentNode.preppend(childNode); //追加子节点（第一个）
siblingNode.before(node); //在指定节点的前面追加元素
siblingNode.after(node); //在指定节点的后面追加元素
```
3. 删除节点
```
node.remove()
```
# 10 . 基于jQuery的Ajax
1. $.get("url",function(data){})
2. $.post()
3. $.ajax({配置参数})