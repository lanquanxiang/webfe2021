选择器
# 1. 常用选择器(4个，掌握，考试)
1. ```*```通配符选择器
> 选中网页中的所有元素
> 作用：清除默认样式
2. 标签选择器 E
> 选中网页中E这个元素
3. id选择器  #id的值
> 选中网页中具有某个id值的元素
> id唯一（不要取纯数字）
4. class选择器 .class的值
> 选中网页中具有某个class值的元素
> 不唯一
> 一个元素可以具有多个class，在class值用空格隔开
# 2. 组合选择器(6个，掌握，考试)
1.  E F 后代选择器
> 选中F
> F是E的后代（包含父子）
2.  E>F 父子选择器
> 选中F
> F必须是E的儿子
3.  E+F 相邻兄弟选择器
> 选中F
> E在F之前，且E和F是兄弟/相邻的
4.  E~F 普通兄弟选择器
> 选中F
> E在F之前，且E和F是兄弟
5.  E,F 或选择器
> 即选中E，也选中F
> int i,k;
6.  E.class  E#id派生选择器
> 选中E，并且E的class等于给定的值
# 3. 属性选择器
1.  存在
```img[width]```
2.  存在且值等于（掌握）
```img[width="600px"]```
3.  存在且值开头匹配 （掌握）   ^= 
4.  存在且值结尾匹配 （掌握）  $=    
5.  存在且值空格分割匹配    ~=
```<div class="t1 t2 t3"></div>```
6.  存在且值连接符分割匹配  |=
```<div class="t1-t2-t3"></div>```
7.  存在且值包含匹配 （掌握）  *=
# 4. 链接伪类
1. :link
2. :visited
3. :hover（掌握）
4. :active
> 顺序：爱（love）恨（hate）原则
> hover鼠标悬停
# 5. 伪元素选择器
1.  首字母    ::first-letter
2.  首行      ::first-line
3.  前面追加  ::before（掌握）
4.  后面追加  ::after（掌握）
```
追加到当前元素的文本中（追加的是子元素）
div:after{
	content:"内容string";
	content:url("资源路径");
}
```
5.  被选中的文字  ::selection
6.  提示文字  ::placeholder（chrome支持）
# 6. 状态伪类
1.  :focus 获得焦点 （掌握）
2.  :not(selector) （开发）
3.  :is(selector) （开发）
4.  :checked 被选中
5.  :disabled 不可用
6.  :read-only 只读
7.  :empty 标签内容为空 （掌握）
> 筛选某一个文本为空的元素
# 7. 结构伪类
1.  E:first-child
> 筛选E元素
> E是老大（E是他父元素的第一个儿子）
2.  E:last-child
3.  E:only-child
4.  E:nth-child(n)（掌握）
> E:nth-child(2n) 偶数odd的孩子
> E:nth-child(2n+1) 奇数even的孩子
5.  E:nth-last-child(n)
6.  E:first-of-type
7.  E:last-of-type
8. E:only-of-type
9. E:nth-of-type(n)
10. E:nth-last-of-type(n)
# 8. 选择器的优先级
