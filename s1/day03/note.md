# 1. 路径的编写【重点，掌握】
1. 绝对路径：路径非常清晰--书写的内容的太多/不便于移动 （第三方资源）
2. 相对路径：路径书写少，便于移动 / 相对关系不能发生变化（相对于当前URL）
	1. 在同一目录下：直接写文件名.扩展名
	2. 在上级目录： ../文件名.扩展名
	3. 在下一级目录： 文件夹名字/文件名.扩展名
3. 相对服务器路径（相对于服务器根路径）： /后续编写路径
	eg. /s1/day02/note.md
# 2. 超链接
1. 语法``` <a href="链接地址" target="打开方式" title="提示" name="命名(书签)">超链接文字</a> ```
2. 打开方式：_blank （新窗口） _self（当前） frame的名字（在指定名称的窗口中打开）
3. 书签链接【简答题，考试】
	1. 使用#链接书签（名字） 
	2. 在书签的位置使用name添加空白a元素/给书签位置的指定元素添加id
# 3. 图片
1. 语法``` <img width="" height="" title="提示" alt="替代文字"/> ```
2. 宽高只需要设置一个
3. 如果同时设置可能会变形
# 4. 表格
1. 语法
2. 合并单元格 rowspan  clospan
3. 扩展：表格的结构标记 thead tbody tfoot(批量的对某几行进行操作)
	