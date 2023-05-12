Ajax
# 1. 概念
1. (A)异步的 JavaScript and XML（数据text、xml、json）
2. 通过异步机制，使用JavaScript（DOM）将XML中的数据显示在网页中（不刷新网页）
# 2. 为什么
1. 异步（提高效率）/同步
2. 无刷新更新页面
# 3. 优缺点
1. 优点：提高效率、节省带宽、降低服务器压力
2. 缺点：URL→多个内容
# 4. text数据
## 1. 同步请求
1. 初始化对象
```var xhr = new XMLHttpRequest();```
2. 创建请求
```xhr.open("请求方式","请求地址",是否异步);```
3. 发送请求
```xhr.send();```
4. 处理响应
```var txt = xhr.responseText;```
## 2. 异步处理
```
xhr.onreadystatechange = function(){
	if(xhr.readyState==4 && xhr.status==200){
		//数据处理
	}
}
```
# 5. xml数据请求
1. xml编写
> 必须有唯一的根节点
> 所有的标签任意命名
> 所有的标签必须成对
> 所有的属性值必须加引
2. xml存储数据
> 存储在属性中 getAttribute()
> 存储在文本中
3. 数据响应
> xhr.responseXML; // XML文档树，对树的操作类似于DOM
# 6. JSON数据请求（JavaScript对象标记）
1. json语法
> {}或者[]
> 名字需要引号，名字:值
> 值可以是任意值（字符串、数组、对象）
2. 格式校验
[JSON格式校验](https://www.bejson.com/)
3. 数据读取
> 以文本的方式读取  jsonstr=xhr.responseText;
> 将文本转为JSON对象
```
obj = JSON.parse(jsonstr);
obj = eval("("+jsonstr+")");
```