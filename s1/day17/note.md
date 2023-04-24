# 1. 增加网页节点（元素）
1. 创建节点
```
var newele = document.createElement("tagname");
```
2. 为节点增加必要的内容（属性、文本） eg.图片src 超链接href和链接文本
3. 将节点添加到网页中
```
	父元素.appendChild(newele); //增加到父元素中，且是父元素的最后一个孩子
	后面的兄弟.parentNode.insertBefore(newele,后面的兄弟); //parentNode节点的父元素
```
# 2. 批量增加节点
1. 使用循环直接增加节点，渲染n次，降低效率
2. 解决：使用文档碎片
```
1. 创建文档碎片
2. 循环创建n个节点，将节点加入文档碎片中
3. 将文档碎片添加到网页中
```
# 3. 删除节点
```
ele.parentNode.removeChild(ele);
```
# 4. BOM
1. document == window.document
2. 常用属性（网址）【重点】
```
window.localtion.href  //读：当前网址；写：改变网址（跳转到新的网页）
```
3. 常用方法
> 打开关闭窗口【了解】
```
var win = window.open("URL");
win.close();
```
> 计时器【重点】
```
1. 周期性执行 var t=setInterval(函数名,毫秒);  clearInterval(t);
2. 一次性执行 var t = setTimeOut(函数名,毫秒);  clearTimeOut(t);
```
* 计时器中的延迟函数，在异步中执行（主函数执行完毕之后再来执行计时器代码）
> 交互框
```
1. 警告框 alert("")
2. 确认框 var boolean =  confirm("quession")
3. 询问框 var string = prompt("问题","默认答案")
```
> 扩展
```
window.history 访问浏览器的历史记录（当前窗口）
document.cookie 读写浏览器cookie
```