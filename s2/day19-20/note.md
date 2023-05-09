# Ajax
## 1. 概述
1. 是什么
> 异步JavaScript和XML（HTML）
> XML：标记数据的结构（数据的传输）
2. 做什么
> 无刷新更新页面
* 局部刷新
* 更新页面内容（服务器、外部资源）
3. 为什么
* 异步：节省时间，提高用户体验
* JavaScript：DOM操作网页元素
* XML：保存更新的内容（txt、xml、json）
4. 优缺点
* 节省带宽，减轻服务器压力
* 提高用户体验
* URL和内容不一致（无法后退、搜索引擎不易收录）
## 2. 如何使用【重点】
1. 创建对象
2. 创建请求 open("get/post",url,是否异步true/false)
3. 发送请求 send()
4. 处理响应（三类数据 text、xml、json 两种情况：同步、异步）
## 3. 处理响应
1. text
* 获得数据 var s = 对象.responseText
* 异步处理（xhr.readystate==4&&xhr.status==200）
2. XML
3. json
## 4. XML
1. 语法
* 所有标签必须成对出现
* 标签任意命名
* 所有属性值必须加引号
* 必须唯一根标记
2. 数据标记
* 将数据标记在文本中
* 将数据标记在属性中
3. 处理响应
* 数据：xhr.responseXML;得到的是一个类似于DOM的对象
## 5. JSON（JS对象）
1. 语法
* [] 数组
* {} 对象
```
{"name":"zhangsan","score":[{"name":"web","s":98},85,87]}
```
[JSON格式校验](https://www.bejson.com/)
2. 数据获得
* 使用str = xhr.responseText得到文本数据
* 将文本转换为JSON对象
> JSON.parse(str)
> eval("("+str+")")
3. 实例