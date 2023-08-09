# 项目介绍

本项目为css及flex布局练手项目，从0仿照百度百科网页介绍一部喜欢的电视剧
整体布局分为header、main-content两大部分，其中header蔚蓝色简介部分。main-content又分为summary、info、actors三大部分。
对于大模块以及模块中图片、并列文字项等处，都使用了flex布局。

# CSS易错点
1.要用reset.css清除样式

2.块级元素子元素继承父元素宽度，所以即便header-inner已经margin:0 auto，依然会撑满整个宽度

3.对vertical-align用的不熟

4.==设置padding会时撑大元素==，大于自己设置的70%width！因此需要直接让父元素宽度为70%

5.如何控制图片宽度一致，高度自由裁剪？设置height为auto

6.如何实现点赞转发那里基本样式相同，但首尾个例样式不同：==:not(:last-child)伪类选择器==

7.阴影效果：box-shadow属性

8.怎么画居中的线：将块元素高度设置为1

9.负margin的应用：用负margin移动标题，使蓝条能占用padding的位置，中间的空白用子元素的padding


# 疑问
1.为什么header的p的margin-top和参考页面设置的一样，实际大小却不一样

2.body的lint-height：1是为了什么

3.为什么info类为flex时横线无法显示