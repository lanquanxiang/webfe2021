# 1. 事件三要素
1. 元素
2. 事件
3. 事件处理程序（响应）
# 2. 事件绑定的方法
1. 在元素的开标签中添加**事件**及**处理程序**
```
<button onclick="fun()">按钮</button>
```
2. 获得元素，然后给元素的**对应事件**绑定**处理程序**
```
document.querySelector("button").onclick = fun;
```
3. 事件监听，获得元素，然后给元素**添加事件监听**，添加事件名称、响应程序、是否捕获型
```
document.querySelector("button").addEventListener("click",fun,true);
document.querySelector("button").removeEventListener("click",fun,true);
```
# 3. 事件对象event（window.event）
1. event.type 事件名称
2. event.target 触发事件的元素
# 4. （了解）事件模型
1. 捕获型
2. 冒泡型
# 5. 鼠标事件
## 1. 常用事件
1. onclick	鼠标单击
2. ondblclick	鼠标双击
3. onmouseenter	鼠标进入元素
4. onmouseover	鼠标悬停元素(会产生事件冒泡）
5. onmouseout	鼠标移出元素
## 2. 冒泡
> event.stopPropagation阻止事件在 DOM 中继续冒泡
# 6. 键盘事件
## 1. 常用事件
1. onkeydown	键盘按下
2. onkeyup	键盘弹起
3. onkeypress	键盘按下并释放
## 2. 常用属性
```
event.keyCode  //键入的ASCII码  97
event.key //键入的字符   a
```
# 7. 编辑事件
```
oncopy
onpaste
```
# 8. 表单事件【重要:对数据进行验证】
1. onsubmit="return fun()"	表单提交 form标签中//需要返回值，false阻止表单提交【重点】
2. onreset	表单重置
3. onchange	内容被改变并失去焦点 //input输入标签中，eg. 判断用户名是否被注册
4. onblur	失去焦点
5. onfocus	获得焦点
# 9. 页面加载事件
onload 页面所有内容加载完毕之后触发
> 数据的初始化
> 运行页面打开之后立即执行的脚本
