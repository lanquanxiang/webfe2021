# 1. html概述
1. html：超文本标记语言
2. 作用：网页的内容和结构
# 2. html特点
1. 不需要编译
2. 解释性语言（由浏览器解释）
3. 不区分大小写（建议小写）
4. 不可见字符解析为空百符
# 3. html结构
## 1. 版本声明
1. html4.01 -> xhtml -> html5
2. 标记的概念
3. html结构标记 html>head+body
	1. head头部：标题+网页头信息
	2. body正文：能够在网页中看见的信息
# 4. 常见标记
## 1. 特殊标记
1. 空格
2. 换行
3. 小于 less than 
4. 大于 great than
5. 小于等于 大于等于 ``` &le;   &ge; ```
6. 版权
7. 水平分割线 hr
## 2. 标题标记
## 3. 标记分类【重点】
1. 块级元素（独占一行，允许设置宽度和高度）  div(容器)
2. 行内元素（共用一行，不允许设置宽度和高度）span(容器)
3. 行内块元素（共用一行，允许设置宽度和高度）eg. img图片标记；css可以进行类型转换
## 4. 修饰文字标记
1. 加粗 blod
2. 斜体 italic
3. 下划线 underline
4. 下划线 ins --> insert
5. 字体font
	1. 长度单位（了解）
	2. 颜色表示方法（掌握）
	   1. 单词red
	   2. #十六进制   rgb 0-255  红色 #FF0000
	   3. CSS能够使用 rgb(255,0,0)函数 rgba(255,0,0,0.5)
## 5. 其他
1. 段落 p 属性align
# 5. 列表
## 1. 有序列表（order list）
1. ol>li
2. type属性改变列表项
## 2. 无序列表（unorder list）
1. ol>li
2. type属性改变列表项
## 3. 嵌套（多级）列表[重点，考试]
二级列表是属于一级列表的列表项
li>ul/ol

