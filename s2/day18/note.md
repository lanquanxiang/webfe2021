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