jQuery
# 1. 概述
1. 是什么？
JavaScript脚本（库）【导入库】
2. 怎么用？
> 下载库
> 导入到网页中
3. 为什么？
提高开发效率
> 获取元素（文本、属性编辑）
> 事件响应
> 节点操作
# 2. DOM[1-7重点]
## 1. 获得节点
> $("css选择器")
## 2. 索引器
> jobj[index] 数组索引，得到DOM对象
> jobj.get(index) 得到DOM对象
> jobj.eq(index) 得到jQuery对象
* 扩展：DOM效率更高
## 3. 修改文本/获取文本
* DOM: obj.innerHTML/innerText
* jQuery: jobj.html()/jobj.text()
## 4. DOM对象（dom）和jQuery（jq）对象互转
* jq = $(dom);
* dom = jq[0]   jq.get(0)
## 5. 获得/修改值
* DOM：obj.value
* jQuery: jobj.val()
## 6. 获得/修改属性
* DOM: obj.set/getAttribute()
* jQuery:jobj.attr()
## 7. 修改css样式
* 设置单个值 jobj.css("样式名","样式值")
* 获取单个值 jobj.css("样式名")
* 设置多个值 jobj.css({CSS样式表})
* 设置某个class jobj.addClass(class名字)
## 扩展
1. 属性attribute：HTML节点属性（网页渲染之后的属性）
2. 属性property：HTML节点对象的属性
## 8. jQuery其他筛选器
* :first
* :last
* :even
* :odd
* :eq(n)
* :le(n)
* :gt(n)
* :empty
* :checked
* :disabled
* :selected
* :表单type 选中指定类型的输入控件
* next(); //当前元素之后的紧邻着的第一个兄弟元素(下一个)
* nextAll();//当前元素之后的所有兄弟元素
* prev();//当前元素之前的紧邻着的兄弟元素(上一个)
* prevAll();//当前元素之前的所有兄弟元素
* siblings();//当前元素的所有兄弟元素(不包括当前兄弟)
* children();当前元素之前的所有孩子
# 2. 事件响应
1. DOM为元素的对应事件添加函数
```
<button>按钮</button>
document.querySelector("button").onclick = fun;

```
```
$("button").click(fun) 【重点】
```
2. DOM为元素添加事件监听
```
<button>按钮</button>
document.querySelector("button").addEventListener("click",fun,是否使用捕获型);
document.querySelector("button").removeEventListener("click",fun,是否使用捕获型);

```
```
$("button").bind("clcik",fun)
$("button").unbind("clcik")
$("button").one("clcik",fun) //一次性的事件
```
3. jQuery事件
* 所有的DOM事件去掉on
* onload load（×）页面（结构+内容）加载完成
* ready 结构加载完成，可以多次使用
# 3. 节点操作
1. 创建节点
```var div = $("<div>123</div>")```
2. 将节点加入网页中
```
append 向父元素追加子元素（最后）
prepend 向父元素追加子元素（最前面）
after 向某个元素追加兄弟（后面）
before向某个元素追加兄弟（前面）
```
3. 将节点删除
```
remove
```
# 4. 基于jQuery的Ajax
1. $("selector").load("URL #信息片段")
2. $.get/post("URL",function(){})
3. $.ajax() //高度集成方法