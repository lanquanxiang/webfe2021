# 1. 路径（地址）【掌握】
## 1. 绝对路径
1. 硬盘上的真实路径
2. 网络上的网络地址
3. 优缺点
	1. 优点：路径清晰、不依赖于引用文件的位置
	2. 缺点：书写内容多、不利于项目移植（硬盘路径）、资源不可控（网络路径）
## 2. 相对路径
1. 将资源放在项目中，相对于引用文件进行定位
2. 优缺点
	1. 优点：书写内容少、方便项目移植
	2. 缺点：依赖于相对位置关系（变化之后路径失效）、相对于引用页面的URL（请求转发）
3. 用法
	1. 同一目录：文件名.后缀名
	2. 下一目录：目录名/文件名.后缀名
	3. 上一目录：../文件名.后缀名
	4. 上述三种用法可以嵌套使用
## 3. 相对服务器路径
1. 以“/”开头，相对于服务器根目录
2. 优点：相对于不会变化的根路径（可以自己配置）
# 2. 超链接（行内元素，双标记）
1. 语法
```
<a href="URL" title="" name="" target="">超链接文本</a>
```
2. 属性
	> name标记书签（信息片段）位置（名字）
	> title鼠标悬停之后显示的文字
	> target：_blank 新窗口（新标签页） _self（当前窗口） frame的名字（指定frame窗口）
3. 书签链接
	> 1. 标记位置 + 为已经存在的元素附加id属性
	> 2. 链接书签 href="#位置名字"
# 3. 图像（行内块元素，单标记）
1. 语法
```
<img src="" alt="" title="" width="" height=""/>
```
2. 属性
	> alt：图像加载失败之后的代替文字
	> title：鼠标悬停之后的提示文字
	> width、height：一般只需要设置一个，同时设置可能会变形
# 4. 表格
1. 用处：少量排版、展示数据
2. 语法：
```
table>caption+(tr>td)+(tr>td)
```
3. 要点：
	> 只能设置行高和列宽
	> 水平对齐align、垂直对齐valign（top、bottom、middle）
	> td==th（文字加粗、居中）
	> 结构标记 thead tbody tfoot（批量操作）
