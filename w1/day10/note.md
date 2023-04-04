浮动定位（位置）
# 1. 浮动
1. 文档流
2. 语法 float:left;right;
3. 掌握
> 1. 脱离文档流
> 2. 扩展：位置？影响？怎么消除影响？
# 2. 定位position
1. position: static;         /*默认原位置，无特殊效果*/
2. position: relative;     /*不脱离文档流，默认原始位置，相对于原位置*/
3. position: absolute;(子绝父相)/*脱离文档流，默认原始位置，相对于有特殊定位的父元素*/
4. position: fixed;        /*脱离文档流，默认原始位置，相对于窗口*/
# 3. 显示display
1. display:block（独占一行，可以设置宽高）
2. display:inline （共用一行，不能设置宽高）
3. display:inline-block（共用一行，能设置宽高）
4. display:none （不显示，文档流中消失）
5. visibility: hidden; （隐藏，文档流不消失）
# 4. 图像边框
1. 必须先设置普通边框
2. 图像边框
> 语法 border-image:url() 30 30 30 30 stretch(拉伸);round;
# 5. 线性渐变
# 6. 滤镜
# 7. 变形与动画
