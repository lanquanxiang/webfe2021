# 1. 获得网页元素element（Node）
1. Live Node = document.getElementById("id")
2. Live Node List = document.getElementsByClassName("class")[下标]
3. Live Node List = document.getElementsByName("name")[下标]
4. Live Node List = document.getElementsByTagName("tagname")[下标]
5. Static Node = document.querySelector("selector")
6. Static Node List = document.querySelectorAll("selector")[下标]
# 2. 获得/修改值和文本
## 1. 值
ele.value   ele.value="新的值"
## 2. 文本
ele.innerHTML/innerText 纯文本  ele.innerHTML/innerText="新的值"
# 3. 获得/修改属性
1. 增加/修改 ele.setAttribute("属性","值");
2. 删除 ele.removeAttribute("属性");
3. 获得 ele.getAttribute("属性");
# 4. Math对象
1. Math.floor(X) 选下取整
2. Math.round(X) 四舍五入
3. Math.ceil(X) 向上取整
4. Math.random() 随机[0-1)之间的数
# 5. Date日期
1. 初始化 new Date() 当前日期
2. 常用方法
补充：
> ```setInterval(fun,mill-time);```
# 6. 数据验证（重点）
1. 是否为空 X==""
2. 是否为数字  isNaN(X)==false 是数字
3. 是否一致 X==Y
4. 长度不能少于6位  X.length<6
5. 复杂验证（手机号码、邮箱、混合密码）正则表达式
# 7. 正则表达式
1. 初始化 
> var a = new Reg();
> var b= /../
2. 通配符
> 指定范围选择[]
> 制定类别选择 . \w \d \n \s
> 制定数量 {x,y}
3. 测试方法（重点）
> reg.test(str)