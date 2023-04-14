# 1. 函数function
1. 使用function关键词来定一个函数 function f(){}
2. 使用var定义一个函数变量 var f = function(){}
3. 使用new来初始化一个函数对象 new Function()
# 2. 函数的调用
1. 函数名();
2. 事件响应来调用  onclick="函数名()"
3. 超链接来调用 ```<a href="javascript:函数名()"></a>```
4. 匿名函数自运行 (function(){})();
# 3. 与Java函数的区别
1. 函数的返回值是否存在，由函数体中的return;
2. 形参不需要声明类型，也不需要var
3. 没有函数重载，函数和参数列表无关
4. 如果函数需要参数，没有传参，参数值undefined；传递了多的参数，多的参数忽略
5. 多个同名函数，以最后一个为准
6. 没有return的函数为变量赋值，变量的值变为undefined
# 4. 获得网页元素(重点)
```
Live Node = document.getElementById("id")
Live Node List = document.getElementsByClassName("class")
Live Node List = document.getElementsByName("name")
Live Node List = document.getElementsByTagName("tagname")
Static Node = document.querySelector("selector")
Static Node List = document.querySelectorAll("selector")
```
# 5. 获得/修改元素信息
1. 修改文本  node.innerHTML   node.innerHTML="新的值"
			node.innerText （纯文本）
2. 修改/获得值  node.value   node.value="新的值"
3. 修改/获得属性 
> node.setAttribute("属性","值")
> node.getAttribute("属性")
> node.removeAttribute("属性")
# 6. 数组
1. 初始化
> ```var a = [默认值,默认值];```
> ```var b = new Array(); //可以在括号中填默认值``` 
2. 区别
> 不限长度，不存在数组越界
> 可以访问不存在的下标，得到的值是undefined
> 可以直接向任意下标写入数据，之前的内容undefined  x[5]  x[10]=1 6-9undefined
> JS可以在数组中保存任意数据类型
3. 常用方法
> A.concat(B) 链接A和B两个数组的元素，不影响A的值，返回连接结构
> A.shift() 删除A中的第一个元素，返回被删除的元素
> A.pop() 删除A中的最后一个元素，返回被删除的元素
> A.unshift(任意元素) 向A的头部插入元素，返回新的数组长度
> A.push(任意元素) 向A的尾部插入元素，返回新的数组长度
4. 数组→字符串
> A.toString()
> A.join("指定字符") 使用指定的字符来连接数组中的所有元素
  ```eg. A.join(",") == A.toString()```
## 7. 常用对象Math
1. floor(X) 向下取整
2. round(X) 四舍五入
3. ceil(X) 向上取整
4. random() [0-1)随机数 
> 计时器
```
	setInterval(fun,mill-time);
```