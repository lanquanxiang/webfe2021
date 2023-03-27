# 1. JavaScript概述
1. JavaScript的构成：标准script、DOM、BOM
2. 作用：事件响应、操作对象
# 2. 【掌握】JS的使用
1. 行内JS（不建议）
2. 内部JS（上课）
> 任意位置写script标签
3. 外部JS（建议Web开发）
> 脚本保存到*.js
> 在网页中使用script标签链接（src）进来
4. 特点
# 3. JavaScript的变量
1. 原型：数字、布尔、字符串、null、undefined
2. 引用类型：数组、日期、自定义对象、函数
3. 变量定义关键词：var
4. 注意变量的作用域及变量提升
# 4. 变量的运算
1. “+”如果操作数的左右存在字符串，变为字符串拼接
2. “-”将操作数左右转换为数字进行运算，true==1，false==0
# 5. 数字
1. 表示方法（十进制、八进制、十六进制、科学计数法）
2. 特殊数字 NaN  无穷大 
3. 小数无法精确表示（|a-b|<1e-16）
# 6. 字符串
1. 引号（单引号或者双引号，注意正确嵌套）
2. 当嵌套比较麻烦的时候，可以使用转义字符
3. 换行的转义字符在网页中可能无效
4. new String()初始化是一个object
5. ""初始化是一个string
# 7. 布尔
1. false true
2. 参与算数运算
# 8. 类型转换
1. 字符串转数字
> parseXXX(string) 可以部分转换
> Number(string) （建议）必须完整转换
> string-0		建议
2. 数字转字符串
> num.toString()  不能转null undefined
> String(num)	建议
> num+""        建议
3. 布尔
> Boolean()
> 5个特殊的false值，其他的都是true