jQuery
# 1. 概述
## 1. 是什么？
JavaScript脚本（外部脚本）、库
## 2. 为什么？
提高**开发**效率：获得网页元素、快捷的常用方法
jQuery是对JavaScript的封装，**执行效率**低于DOM
## 3. 怎么用？
1. 下载脚本 [https://jquery.com/download/](https://jquery.com/download/)
2. 链接外部脚本到网页中
```
<script src="js/jquery-3.7.0.js"></script>
```
## 4. 有什么？
通过**指定元素**的**事件响应**来控制网页中的元素（**查改增删**）
# 2. 获得指定元素
## 1. 选择器
```
$("选择器/筛选器")
eg. $("div")  $("#idname") $(".classname")
```
注意：如果是多个，也可以直接进行操作（操作每一个元素）
## 2. 索引器（在很多个被选中的元素中找到指定的元素）
```
jobjs.eq(index)   //jQuery对象
jobjs.get(index)  jobjs[index]    //DOM对象
```
## 3. 对象的转换
DOM对象 = jQuery对象[0]
jQuery对象 = $(DOM对象)

# 3. 事件响应
1. 触发事件
```
1. 获得元素(按钮)
2. 调用元素的对应事件函数
$("button").click(fun);
```
2. 事件
在DOM事件基础上去掉“on”
> 扩展：对象不发生变化，可以连续调用方法（链式语法风格）
> onload 页面加载之后触发 load(×) ready()
onload:只能使用一次，页面加载（结构html标签+内容：资源）
ready：可以使用多次，文档准备就绪（结构html标签）
3. 事件绑定
```
$("button").bind("click",fun);
$("button").one("click",fun); //执行一次之后失效
$("button").unbind("click");
```

# 4. 操作元素
## 1. 对元素进行修改/获得
### 1. 文本
```
dom.innerHTML/innerText
jquey.html()/text()		jquery.html(新的值)
```
### 2. 属性
```
dom.getAttribute("属性名")  dom.setAttribute("属性名","值")
jquery.attr("属性名")  jquery.attr("属性名","值") 
```
1. 文本框的值
```
dom.value    	dom.value="新的值"
jquery.val()	jquery.val("新的值")
```
2. 单选、多选、下拉列表的选中
```
判断  is(":checked")
改变值 $("selector").prop("checked",false/true);
property属性（页面节点对象的属性）    prop()
attribute属性（页面渲染之后的节点属性） attr()
```
### 3. CSS（jQuery）
```
jquery.css("样式名","样式值");
jquery.css({"样式名":"样式值","样式名":"样式值","样式名":"样式值"});
jquery.addClass("类名")   //需要现在网页中定义css样式表（class样式表）
jquery.removeClass("类名")
```
## 2. 对元素进行增加和删除
1. 创建元素
```
$("网页元素")
```
2. 添加元素到网页中
```
parenode.append(newnode) 将新节点追加到某个元素中（最后一个孩子）
parenode.preppend(newnode) 将新节点追加到某个元素中（第一个孩子）
siblingnode.before(newnode)将 新节点追加到某个元素之前（兄弟）
siblingnode.after(newnode)将 新节点追加到某个元素之后（兄弟）
```
3. 删除
```
curnode.remove()
```
# 5. 基于jQuery的Ajax
```
$("selector").load("url #信息片段")   // 了解

$.get/post("url",{data},function(data){处理数据data})

$.ajax({
	url:"",//请求地址
	data:"",//传递给服务器的数据
	type:"get/post",//请求方式
	async:false/true,//同步异步
	dataType:"text/xml/json",//响应的数据类型
	success:function(data){},//成功的回调函数
	error:function(data){}	//成功的回调函数
})

```
# 6. 动画
1. 显示和隐藏  jquery.hide()/show()
2. 淡入淡出   fadeIn()/fadeOut()
3. 划入划出  slideDown()/slideUp()
4. 停止动画 stop()
5. 自动动画 animate
# 7. 模拟用户操作
```
$("button").click(); //不加参数，表示模拟操作
```