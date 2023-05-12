Ajax
# 1. 概述
## 1. 是什么？
异步的（A）JavaScript and XML（数据txt、xml、json）
## 2. 有什么用？
通过同步/异步方式，使用JavaScript（DOM）将数据（服务器）更新在页面上
## 3. 为什么？
无刷新更新页面
> 局部更新（节省带宽、减轻服务器压力）
> URL--> 资源（变化）、不方便搜索引擎搜索
# 2. txt数据
## 1. 同步操作
1. 创建 XMLHttpRequest 对象
```var xhr = new XMLHttpRequest();```
2. 创建URL请求
```xhr.open("get/post",url,"是否是异步true/false同步");```
3. 发送请求
```xhr.send();```
4. 处理响应信息(接收数据、解析数据、DOM显示数据)
> 文本信息：xhr.responseText;
## 2. 异步操作
```
xhr.onreadystatechange=function(){
	if(xhr.readyState==4 && xhr.status==200){
		//处理数据		
	}
}
```
# 3. XML数据
1. XML语法
> 唯一的根标记
> 标记的名字任意命名
> 标签必须成对
> 标签的属性值必须加引号
2. 书写方法（文本、属性）
3. 数据解析
> getAttribute
> innerHTML/innerText
# 4. JSON数据（JavaScript object noted）
1. json语法
> [],{}
> 对象：属性必须加引号，属性和属性值之间用冒号，多个属性之间用逗号
```
[
{
	"name":"zhangsan",
	"sno":"202101",
	"scores":[
		{
			"course":"web前端",
			"score":100
		},
		{
			"course":"数据结构",
			"score":101
		}
	]
},
{
	"name":"zhangsan",
	"sno":"202101",
	"scores":[
		{
			"course":"web前端",
			"score":100
		},
		{
			"course":"数据结构",
			"score":101
		}
	]
}
]
```
2. 校验格式
[JSON校验](https://www.bejson.com/)