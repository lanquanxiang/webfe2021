选择器
# 1. 常用选择器（掌握）
## 1. *通配符
1. 选中的是所有元素
2. 清除默认样式
## 2. 标记选择器（类型选择器）
1. 直接按照标记进行选中
2. 一般适用于基础样式
## 3. id选择器（重要）
1. 选中具有特定id值的元素（唯一）
2. ```#id的值{声明}```
## 4. class选择器(重要，常用)
1. 选中具有相同class的元素（不唯一）
2. ```.class的值{声明}```
# 2. 组合选择器（掌握）
> 增加选择器的权重
## 1.  E F 后代选择器
> 选中的F这个元素
> 且F必须是E的后代
## 2.  E>F 父子选择器
> 选中F这个元素
> 且F是E的儿子
## 3.  E+F 相邻兄弟选择器
> 选中F这个元素
> 且E元素在F元素之前，他们是相邻的兄弟
## 4.  E~F 普通兄弟选择器
> 选中F这个元素
> 且E元素在F元素之前，他们可以不相邻
## 5.  E,F 或选择器
> 选中E，或者F
> 作用：对多种选择器同时进行声明    int i,j,k;
## 6.  E.class E#id派生选择器
> 选中E元素，且该元素的class等于给定值
# 3. 属性选择器
1.  存在
2.  存在且值等于    = （重要）
3.  存在且值开头匹配    ^=  （重要）
4.  存在且值结尾匹配    $=   （重要） 
5.  存在且值空格分割匹配    ~=
6.  存在且值连接符分割匹配  |=
7.  存在且值包含匹配    *=
# 4. 链接伪类(超链接)
> 爱(love)恨(hate)原则
> a:link (链接之前的样式)
> a:visited （点击之后的样式）
> a:hover (鼠标悬停的样式)（掌握）
> a:active （点击的一瞬间（激活））
# 5. 伪元素选择器(6种)
1.  首字母    ::first-letter
2.  首行        ::first-line
3.  前面追加  ::before（重要）
4.  后面追加  ::after（重要）
```
			div::before{
				content: url(img/excel.png); /*追加图标*/
				content: "xxxx"; /*追加文字*/
			}
```
5.  被选中的文字  ::selection
6.  提示文字  ::placeholder
> 当选择器权重一样时，越靠近元素的优先级越高。
# 6. 状态伪类选择器(7种)
1.  :focus 获得焦点
2.  :not(selector)
3.  :is(selector)
4.  :checked 被选中
5.  :disabled 不可用
6.  :read-only 只读
7.  :empty 标签内容为空
# 7. 结构伪类选择器(10种)
1.  E:first-child
2.  E:last-child
3.  E:only-child
4.  E:nth-child(n)
> 2n,odd,even
5.  E:nth-last-child(n)
> 选中的是E，且符合E是其父元素的第几个儿子
6.  E:first-of-type
7.  E:last-of-type
8. E:only-of-type
9. E:nth-of-type(n)
10. E:nth-last-of-type(n)
# 优先级【重要】
