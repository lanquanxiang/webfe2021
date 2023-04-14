# 函数
## 1. 函数的定义
1. 使用function关键字声明函数
2. 使用var来初始化一个函数变量
3. 使用new Function()的构造方法构造函数
## 2. 注意
1. 不需要设置返回值，是否有返回值由函数体中的return
2. 函数形参中不需要使用var  eg. function max(i,j)
3. 函数可以重复定义，而且没有函数重载  eg. function max(i)
4. 函数形参个数不固定，缺少形参，形参的值是undefined，多的形参忽略
5. 如果使用了没有返回值的函数为变量赋值，变量的值undefined
## 3. 常用的全局函数
1. isNaN(X) : 判断用户输入的是否为数字 false
2. eval("code") ： 运算字符串的值
3. encodeURI(X)/decodeURI(X) : 编码解码地址栏的中文；读写cookie[不允许保存中文]
