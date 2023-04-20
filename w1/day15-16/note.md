# 1. 字符串
1. 初始化
```
var s1 = ""; //原型 string
var s2 = new String(); //引用类型 object
```
2. 常用方法
	1. str.length
	2. 位置→字符  charAt(index)  str[index]
	3. 字符→位置	 indexOf("字符") //第一个字符 lastIndexOf() 最后一个字符;如果未找到，返回-1
	4. 字符串截取 str.substring([start,end)) str.substr(start,length); 如果省略第二个参数，默认截取后续所有字符
	5. 字符串→数组	str.split("字符") 如果字符为""，每个字符都是一个数组元素
# 2. 自定义对象
1. 初始化
```
var obj = {};
```
2. 对象属性(JSON)
```
var stu = {sno:"202110803001",age:18}
stu.name = "zhangsan";
stu["school"]="pzhu";
```
3. 属性访问
```
obj.属性名  //如果读取了对象不存在的属性，得到undefined
obj["属性名"]
obj.函数属性(); //运行函数
```
# 3. URL编码解码
1. 编码 encodeURI("X")
> URL中包含中文或特殊字符 
> cookie保存中文或特殊字符
2. 解码 decodeURI("X")
# 4. 日期Date
1. 初始化
```
var d1 = new Date(); // 当前日期
var d2 = new Date("2023-04-20T09:10:10"); //初始化指定日期
```
2. 常用方法
# 5. 验证用户数据（重要）
1. 验证数据是否为空 if(x=="")
2. 验证两次数据是否一致 if(x!=Y)
3. 验证数据是都是数字  if(isNaN(x))
4. 验证数据的长度  if(x.length<6)
5. 验证数据的格式（复杂验证） !reg.test(str) //reg正则对象
# 6. 正则表达式（简单能写，复杂能看）
1. 初始化
```
var reg1 = /.../;
var reg2 = new Reg(/.../);
```
2. 字符类别
> \d 数字
> \w 数字、字母或下划线
> \s 空白符
> \n 换行符
> . 任意字符
> [5-9] [a-z] [A-Z] [A-z] [a-zA-Z]范围限定
> (x|y|z) 在列表中选择
> \. \? \+转义字符
3. 量词
> * 任意个 {0,}
> ? 最多一个 {0,1}
> + 至少一个 {1,}
> {x} x个
> {x,y} 至少x个，最多y个
4. 限定符
> ^ 字符开始
> $ 字符结尾
> /reg/i 忽略大小写
> /reg/g 全局匹配