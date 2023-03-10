# 1. 下拉列表
1. 作用：单选、多选框-->太多的时候-->下拉列表
2. 语法：select>option
3. 属性：
> select : name 下拉列表的名字
> select : size 一次可见的数量
> select : multiple 允许多选
> option : value 选项的值
> option : selected 默认选中

# 2. 文本区域标记
1. 作用：文本框-->输入大量的内容-->多行文本（文本区域标记）
2. 区别：双标记
3. 语法：``` <textarea rows="" cols=""></textarea> ```
4. 属性
> rows 行
> cols 列（字符）
> 在标签中间的文本中添加默认值

# 3. 按钮
1. button标记
2. 在使用的时候建议添加type属性
> button:普通按钮
> submit：提交按钮
> reset：重置按钮
3. 在form以外常用标记

# 扩展（了解）：
1. 表单说明 ： form > fieldset > (legend + 其他表单控件)
2. 扩大焦点：
> 1. 给获得焦点的控件附加id
> 2. 给点击的元素 lable中，for属性链接id
