# 1. 表单的概念
1. 收集用户数据
2. 表单标记 form
# 2. 表单用法【重要，考试，编程题】
```
<form action="" method="" ectype="" target="" name="" > 
	表单内容
</form>
```
1. action="URL" 表单的提交去向，数据处理地址
2. method提交方式 get/post【简答题，面试】
	1. get 数据直接显示在URL中；post将数据放在请求实体中；
	2. get数据长度有限制；post没有限制
	3. get请求+数据一起传输；先发请求等待服务器响应（1XX），再发数据；
	4. get：可以数据保存书签，允许缓存，多次提交不影响结果；post：不能存书签，不能缓存，多次提交可能影响结果。
	5. 特殊数据，如图像，文件等，必须使用post
3. ectype编码方式
	1. 一般不需要设置
	2. 当进行文件上传的时候，必须设置 multipart/form-data
4. name 表单的名字
	1. 一般也不需要设置
	2. 可以通过名字来获取表单的值（JavaScript）
# 3. 表单的控件【重要，考试，编程题】
1. 输入控件```<input type=""/>```（HTML4.01 10个 html5 10+（5个））
2. 下拉列表
3. 文本区域标记
4. 按钮
# 4. 输入控件
1. text文本框属性
	1. name名字（参数名字，框里面的值就是参数的值）
	2. value（默认值）
	3. size大小
2. submit属性
	1. name不需要
	2. value 按钮上面的文字
3. 隐藏域（用户不可见，传输默认数据）
	1. 需要传输默认数据
	2. 和不可用的字段（disabled属性）一起连用
4. 单选按钮
	1. 同一组单选必须设置相同的name值
	2. 用户直接选择的，必须提供内（服务器）外（用户）两种值