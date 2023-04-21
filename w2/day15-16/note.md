# 1. 字符串String
1. 初始化
```
var s1 = "abc"; //原型 string
var s2 = new String("abc"); //引用类型 object
```
2. 常用方法
> 长度 s.length
> 字符→位置   s.indexOf("字符") 第一次出现的位置，未找到返回-1；位置从0开始
> 字符→位置   s.lastindexOf("字符") 最后一次
> 位置→字符	s.charAt(index) s[index]
> 字符串截取
	1. s.substring([start,end)) //如果省略第二个参数，默认截取后续所有字符
	2. s.substr([start],length)
> 字符串拼接  a+b
> 字符串→数组   s.split("字符") //参数是""，每个字符分割为一个数组元素
# 2. 自定义对象
1. 初始化
```
var obj= {};
```
2. 属性(成员变量)
```
var obj={name:"value",name:"value"}
obj[name2]="value"
```
eg.
```
var stu={sno:"202110000000",name:"zhangsan",print:function(){}}
stu["school"]="pzhu";
```
3. 访问
```
stu.sno  // 如果属性不存在，得到undefined
stu["name"]
stu.print();
```
# 3. URL编码解码
1. 编码encodeURI(X)
> URL参数中包含中文或特殊字符
> 使用cookie保存中文或特殊字符
2. 解码decodeURI(X)
# 4. Date日期对象
1. 初始化
```
var date1 = new Date(); //当前日期
var date2 = new Date("2023-04-21T09:22:40");
```
2. 常用方法
> 获得年月日时分秒、星期
> 日期→字符串
3. 扩展
> setInterval(函数名,毫秒);
# 5. 数据验证（重点）
1. 信息不能为空 if(x=="") return;
2. 信息一致性（密码==确认密码） if(x!=y) return;
3. 信息长度限制（密码不能少于6位） if(x.length<6) return;
4. 信息必须是数字（评分） if(isNaN(x)) return;
5. 正则表达式验证复杂规则
# 6. 正则表达式
1. 初始化
```
var reg1 = /.../;
var reg2 = new RegExp();
```
2. 语法
>字符类别
```
\d 数字
\s 空白符
\w 数字、字母或下划线
\n 换行 
. 任意字符
[6-9][a-z][A-Z][A-z][a-zA-Z]
(x|y|z)
```
> 量词
```
{n} n个
{0,n} 最多n个
{n,} 最少n个
{n,m} 最少n个，最多m个
+ == {1,}
? == {0,1}
* == {0,}
```
3. 限定符
```
^ 开始符
$ 结束符
/i 忽略大小写
/g 全局搜索/替换
```
4. 使用正则验证
```
reg.test(x)    
/\d{1,3}/
```