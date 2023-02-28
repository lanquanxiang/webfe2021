# 表单
作用：收集用户信息
# 1. 语法
1. 格式【考试，编程题】
```
<form action="" method="" enctype="" name="" target="">
	表单的内容//表单控件
</form>
```
2. 属性
 1. action = "URI" 表单的提交地址
 2. method = "get/post" 默认get：提交方式
	> 扩展：区别【面试，简答题】
	> 1. get将数据显示在URL中；post将数据封装在http的实体中
	> 2. get有数据大小的限制；post没有限制，实体大小没有限制
	> 3. get保存提交的数据，能够缓存，能够存书签；post的数据不能缓存，不能存书签
	> 4. get多次提交不影响结果；post多次提交可能会影响结果，浏览器会警告提示
	> 5. get 请求+数据 一起传送；post 请求->服务通知（1XX）继续传送数据->在传输数据
	> 6. get需要注意数据的编码（URL只支持ASCII）URL编码；post 实体编码
	> 7. 如果文件上传，必须使用post
 3. enctype（编码类型）
  > 1. 一般情况下不需要设置
  > 2. 文件上传的时候，必须要设置 multipart/form-data
 4. name属性为表单命名，可以通过名字空间来获取表单中的值
# 2. 表单控件
1. input输入控件（HTML4.01 10种，html5 5种）
2. select下拉列表
3. textarea文本区域标记（多行文本）
4. button 按钮 ```<button>按钮</button>```
# 3. 输入控件类型
1. 语法
```
	<input type="类型" name="参数名" value="默认值"/>
```
类型：
> 四个框（文本框text、密码框password、单选框radio、多选框checkbox）
> 四个按钮（普通按钮button、重置按钮reset、提交submit、图像提交按钮image）
> 两个域（文件域file、隐藏域hidden）
2. text
> 默认值 value
> 提示语 placeholder
> 必须name属性
3. submit
> value表示按钮上的文字
4. hidden
> 1. 需要传递默认值 + 传递被disabled禁用的值
> 2. name：默认的参数名
> 3. value：默认的参数值
5. 单选框
> 1. 用户直接点选的控件，必须设置内部值（value-服务器）和外部值（用户）
> 2. 同一组单选必须有相同的name
> 3. 属性checked默认选中
> 4. 属性disabled不可用：用户不能修改，服务器不可读取
> 5. 属性readonly只读：用户不能修改，服务器可以读取
6. 多选
> 1. 第一点同上
> 2. 第二点可选