# 1. 路径
## 1. 绝对路径：硬盘的真实路径（×）/网络URL（√）：第三方资源
> 书写内容太多
> 资源属于第三方，资源不可控
## 2. 相对路径：项目内部【掌握】
> 资源需要添加到项目中
> 只需要书写相对位置关系
>用法
1. 同一目录：文件名.后缀名
2. 下一目录：文件夹名字/文件名.后缀名
3. 上一目录：../文件名.后缀名
4. 嵌套使用
## 3. 相对服务器路径（只限定于服务器内部）【掌握】
1. 相对于服务根路径
2. 不依赖于当前页面位置
3. 用法：以/开头，标识根路径
# 2. 超链接(行内元素)
1. 语法 ```<a href="">链接文字</a>```
2. 属性
> href:链接地址（路径）
> title：鼠标悬停的提示文字
> target: _self(当前窗口)、_blank（新窗口、新选项卡、标签页）、frame的名字（指定名字的窗口打开）
> name：命名（书签）信息片段（书签定位）
3. 书签链接
> 标记书签位置（name、可以在已经存在的元素上使用id进行标记）
> 在其他需要的地方链接到书签
# 3. 图像（单标记，行内块元素）
1. 语法```<img src=""/>```
2. 属性
> title：提示文字
> alt：图像加载失败之后的代替文字
> width、height：只需要设置（同比缩放），同时设置可能会变形
# 4. 表格
1. 作用：
> 1. 排版（简单）
> 2. 展示大量数据
2. 语法【掌握】table>tr>td
3. 属性
> 1. 垂直对齐
> 2. 只有行才能设置高度，只有列才能设置宽度
> 3. [重要]合并行和列
4. 结构标记：批量操作行 thead tbody tfoot

