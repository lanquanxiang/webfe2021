# 1. DOM（增删改查）
## 1. 查询（6种方法）
## 2. 修改（修改文本、修改属性）
## 3. 增加
1. 增加任意元素（节点）[每增加一个节点，DOM树重新渲染一次]
```
1. 创建元素 var temp = document.createElement("元素的标签");
2. 为元素增加必要的文本或属性 
3. 将元素添加到网页中 父节点.appendChild(temp); // 追加的temp是父元素的孩子（最后）
扩展：后续兄弟节点.parentNode.insertBefore(temp,后续兄弟节点); //追加temp到后续兄弟的前面
```
2. 批量增加节点【提高效率】
```
1. 创建文档碎片
2. 创建n个节点，并将n个节点加入到碎片中
3. 将碎片加入到网页中（在此处只刷新了一次）
```
## 4. 删除
```
temp.parentNode.removeChild(temp);
```
# 2. BOM
## 1. 重要的属性
```window.location.href```
1. 读：得到的是当前URL（网站识别）
2. 写：指定浏览器跳转到某个URL（网页跳转）
## 2. 窗口的打开和关闭
1. var w =  window.open("URL")
2. window.close(w);
## 3. 交互框
1. window.alert("警告内容")  //只有确定
2. var boolean = confirm("确认内容") //确定、取消
3. var string = prompt("询问的问题","默认回答"); //返回回答的字符串
## 4. 计时器
1. 周期性执行
```
var T = setInterval(函数名,毫秒);
clearInterval(T);
扩展：t相当于计时器的id，一般情况下是自增的
```
2. 一次性执行
```
var T = setTimeOut(函数名,毫秒);
clearTimeOut(T);
```
3. JS执行机制
所有计时器函数代码，异步执行（主方法中的代码执行完毕之后才会执行计时器代码）