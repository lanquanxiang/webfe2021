# 1. 事件模型
## 1. 三要素
1. 网页元素
2. 事件
3. 事件响应程序
## 2. 事件处理程序的绑定
1. 事件响应
```
<button onclick="fun()">按钮</button>
```
2. 事件绑定
```
1. 获得元素(按钮)
2. 给元素的对应事件附加函数
document.querySelector("button").onclick = fun;
```
3. 事件监听
```
1. 获得元素
2. 给元素附加被监听的【事件名称】以及对应的处理程序
document.querySelector("button").addEventListener("click",fun,true);
document.querySelector("button").removeEventListener("click",fun,true);
```
## 3. 事件对象
1. window.event 事件
2. event.target 元素
3. event.type 事件名称
4. 事件模型：捕获型、冒泡型
# 2. 常见事件
## 1. 鼠标
1. onclick 单击
2. ondblclcik 双击
3. onmouseover 鼠标悬停
4. onmouseout 鼠标离开
5. onmouseenter 鼠标进入 （×）
## 2. 键盘
1. onkeydown	键盘按下
2. onkeyup	键盘弹起
3. onkeypress	键盘按下并释放（√）
> evnet.keyCode
> 注意：需要禁止默认事件，防止事件阻止失效event.preventDefault();
## 3. 表单事件
1. 编辑事件
> oncopy 复制
> onpaste 粘贴
2. 表单事件（重要）
> onsubmit="return fun()" 表单提交之前出发（有返回值）
  返回值为true，提交表单；否则，禁止表单提交
> onchange 值被改变并且失去焦点
> onblur 失去焦点
## 4. 页面加载事件
1. onload
2. 一般用于初始化数据，或者是页面加载之后自动运行脚本
