# 1. 事件三要素
1. 元素 eg. button
2. 事件 eg. click
3. 处理程序 eg. function fun(){}
# 2. 事件响应
1. 在开标签中添加事件响应
```
<button onclick="fun()">按钮</button>
```
2. 为元素的对应事件添加函数
```
<button>按钮</button>
document.querySelector("button").onclick = fun;

```
# 3. 事件对象event
1. 元素 window.event.target
2. 事件名称 window.event.type
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
3. onkeypress	键盘按下并释放【掌握】
扩展：event.keyCode 按键的ASCII
扩展：event.preventDefault();//取消默认事件
## 3. 编辑事件
1. oncopy 复制
2. onpaste 粘贴
## 4. 表单事件
1. onsubmit	表单提交【掌握】//需要返回值
2. onreset	表单重置（了解）
3. onchange	内容被改变并失去焦点【掌握】
4. onblur	失去焦点
5. onfocus	获得焦点
