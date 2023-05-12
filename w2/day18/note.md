# 1. 事件三要素
1. 元素（事件源） eg. button 
2. 事件		eg. click
3. 响应处理程序 function(){}
# 2. 事件响应
1. 开标签中添加事件
```
<button onclick="fun()">按钮</button>
```
2. 为元素的对应事件绑定函数(灵活的获取任意元素，将HTML与JS分离)
```
1. 得到元素
2. 为元素的对应事件绑定函数
<button>按钮</button>
document.querySelector("button").onclick = fun;
```
3. 为元素添加事件监听（自定义事件模型、可以取消监听）
```
<button>按钮</button>
document.querySelector("button").addEventListener("click",fun,true);
document.querySelector("button").removeEventListener("click",fun,true);

```
> 事件模型：捕获型、冒泡型
# 3. 事件对象 window.event
1. 元素（事件源） event.target
2. 事件名称 event.type
# 4. 常用事件
## 1. 鼠标事件
1. onclick	鼠标单击
2. ondblclick	鼠标双击
3. onmouseenter	鼠标进入元素
4. onmouseover	鼠标悬停元素(会产生事件冒泡）
5. onmouseout	鼠标移出元素
## 2. 键盘事件
1. onkeydown	键盘按下
2. onkeyup	键盘弹起
3. onkeypress	键盘按下并释放
扩展：event.keyCode
## 3. 编辑事件
1. oncopy
2. onpaste
3. onsubmit
4. onchange
## 4. 页面事件
onload 页面内容加载完成之后触发
> 初始化数据
> 页面加载完毕之后自动运行的脚本