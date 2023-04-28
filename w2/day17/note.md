# 1. DOM(元素、节点)
## 1. 增加
```
1. 创建元素  var temp = document.createElement("tagname");
2. 为元素增加必要的属性或文本
3. 将元素添加到网页中  父节点.appendChild(temp); //父元素的最后一个孩子
扩展：追加到某个元素（兄弟）的前面   后续兄弟元素.parentNode.insertBefore(temp,后续兄弟元素)
```
> 每增加一个节点，网页就要重新渲染一次
### 扩展：批量增加节点
```
1. 创建文档碎片
2. 创建元素，并将元素增加到文档碎片中
3. 将文档碎片加入到网页中（只刷新一次，提高效率）
```
## 2. 删除
```
1. 找到需要删除的节点 temp
2. temp.parentNode.removeChild(temp);
```
## 3. 查找
> 6种方法（id、class、name、tagname、css选择器）
## 4. 修改
> 修改文本 innerHTML、innerText
> 修改属性 setAttribute()
# 2. BOM(window)
## 1. 属性
1. window.document
2. window.location.href 当前窗口的URL
> 读：得到当前网址，判断某些脚本是否需要运行
> 写：更改当前网址，网页跳转
## 2. 打开和关闭窗口
1. 打开窗口 var w =  window.open("url","其他窗口的特征值设置")
2. 关闭窗口 window.close(w);
## 3. 交互框
1. 警告框 alert("警告内容！");
2. 确认框 var boolean = confirm("确认的内容?"); eg. 是否确认删除？
3. 询问框 var string  = prompt("问题：","默认答案");
## 4. 计时器
1. 周期性执行
```
var t =  setInterval(函数名,周期性间隔时间-毫秒);
clearInterval(t);
```
2. 一次性执行
```
var t =  setTimeOut(函数名,延迟时间-毫秒);
clearTimeOut(t);
```
3. 扩展知识
> 计时器的句柄t自增的变量
> 计时器代码都需要等待主方法中的代码执行完毕之后在执行