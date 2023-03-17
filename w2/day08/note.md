选择器
# 1. 常用选择器（4个，掌握）
1. *通配符选择器
> 选中网页中所有的元素
> 清除所有元素的默认样式
2. E标签选择器
> E表示html中所有的标签
3. id选择器(#id值)
> 选中具有特定id值的元素
> id是唯一
4. class选择器(.class值)(最常用)
> 选中具有特定class值的元素
> class不唯一，同一个元素可以有多个class值
# 2. 组合选择器(6个,掌握)
1.  E F 后代选择器
> 选中F
> F必须是E的后代（包含在F中）
2.  E>F 父子选择器
> 选中F
> F必须是E的儿子（F的子元素）
3.  E+F 相邻兄弟选择器
> 选中F
> E在F之前，且E和F是兄弟，必须相邻
4.  E~F 普通（通用）兄弟选择器
> 选中F
> E在F之前，且E和F是兄弟
5.  E,F 或选择器（同时声明）
> 选中E，选中F  （int i,j,k;）
6.  E.class  E#id派生选择器
> 选中E，并且E具有指定class值
# 3. 属性选择器
1.  存在 	```img[width]```
2.  存在且值等于(掌握)  ```input[type="text"]```
3.  存在且值开头匹配(掌握)    ```input[type^="t"]``` 
4.  存在且值结尾匹配(掌握)    $=    
5.  存在且值空格分割匹配    ~=
6.  存在且值连接符(-)分割匹配  |=
7.  存在且值包含匹配(掌握)    *=
# 4. 链接伪类
1. :link
2. :visited
3. :hover(鼠标悬停)(掌握)
4. :active
> 顺序爱（love）恨（hate）原则
# 5. 伪元素选择器
1.  首字母    ::first-letter
2.  首行      ::first-line
3.  前面追加  ::before(掌握)
4.  后面追加  ::after(掌握)
5.  被选中的文字  ::selection
6.  提示文字  ::placeholder（chrome支持）
# 6. 状态伪类
1.  :focus(掌握) 获得焦点
2.  :not(selector)
3.  :is(selector)
4.  :checked 被选中
5.  :disabled 不可用
6.  :read-only 只读
7.  :empty(掌握) 标签内容为空
# 7. 结构伪类
1.  E:first-child
> 选中E
> E是他父元素的第一个孩子
2.  E:last-child
3.  E:only-child
4.  E:nth-child(n)  (掌握) 
5.  E:nth-last-child(n)  (掌握) 
6.  E:first-of-type
7.  E:last-of-type
8. E:only-of-type
9. E:nth-of-type(n)
10. E:nth-last-of-type(n)
# 8. 优先级