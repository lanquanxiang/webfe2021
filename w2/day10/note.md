修改元素的位置
# 1. 浮动
1. 文档流
2. 特点：
> float:left;right;
> 脱离文档流
> 漂浮：左、右
3. 影响
> 1. 影响后续元素排版
> 2. 父元素高度坍塌
# 2. 定位position
1. position: static;  /*默认原位置，无特殊效果*/
2. position: relative; /*不脱离文档流，默认原始位置，相对于原位置*/
3. position: absolute;/*脱离文档流，默认原始位置，相对于有特殊定位的父元素*/
4. position: fixed;   /*脱离文档流，默认原始位置，相对于窗口*/
# 3. 显示display
1. 切换元素显示方式（块元素、行内元素、行内块元素）
2. none 让元素消失
