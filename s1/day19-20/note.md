Ajax
# 1. 概述
## 1. 是什么？
（A）异步的 JavaScript and XML（数据的结构）
## 2. 有什么？
使用JavaScript（DOM）将外部数据（XML、txt、JSON）异步的显示在网页中
## 3. 为什么？
1. 将数据和显示分离（选择地址的下拉列表（列表和数据分开））
2. 无刷新更新页面
> 按需更新，减轻服务器压力，节省带宽
> 提高效率
> Ajax安全隐患
> URL对应不同的内容
# 2. 使用Ajax【重点】
## 1. txt数据请求
1. 同步
* 创建 XMLHttpRequest 对象
```var xhr = new XMLHttpRequest();```
* 创建URL请求
```xhr.open("get/post",数据地址,true异步/false同步);```
* 发送请求
```xhr.send();```
* 处理响应信息
> 接收数据 ```var txt = xhr.responseText;```
> 解析数据
> 将数据显示在页面上
2. 异步
```
xhr.onreadystatechange = function(){
	//4(请求已完成)  200 服务器正常
	if(xhr.readyState==4 && xhr.status==200){
		//数据处理
	}
}	
```
## 2. XML请求
1. XML编写规则
> 必须要有唯一的根标记
> 所有的标记必须是成对出现的
> 标记的属性必须加引号
> 所有的标记都是自定义的
2. 数据存储
> 属性
> 文本
3. 接收数据
```var xmldom = xhr.responseXML;```
4. 解析属性数据和文本数据
5. 扩展：动态为下拉列表添加选项
## 3. JSON请求（JavaScript object noted）
1. JSON编写规则
> {},[]
> ["",{},""]
> {"属性":"属性值","属性":"属性值"}
```
{
	"sno":"202110804001",
	"sname":"zhangsan",
	"scores":[
		{
			"course":"web前端",
			"score":100
		},
		{
			"course":"Java",
			"score":101
		}
	]
}
```
2. 接收数据
> var jsonstr = xhr.responseText;
> 将纯文本解析为JSON对象
```
obj = JSON.parse(jsonstr);
obj = eval("("+jsonstr+")");
```