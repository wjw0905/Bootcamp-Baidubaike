# 项目收获

本项目为css及flex布局练手项目，从0仿照百度百科网页介绍一部喜欢的电视剧<br>
整体布局分为header、main-content两大部分，其中header为蓝色简介部分；main-content又分为summary、info、actors三大部分。<br>
对于大模块的分布以及模块中图片、文字项、图文排版等处，都使用了flex布局。<br>
对以下知识点加深了认识：min-width、盒子模型、box-shadow阴影属性、flex-basis(虽然还是再用width)、align-items用于垂直居中、justify-content横向对齐、伪类选择器not(:last-child)

# 具体CSS易错点
1.要用reset.css清<br>
2.块级元素子元素继承父元素宽度，所以即便header-inner已经margin:0 auto，依然会撑满整个宽度<br>
4.==设置padding会时撑大元素==，大于自己设置的70%width！因此需要直接让父元素宽度为70%<br>
5.如何控制图片宽度一致，高度自由裁剪？设置height为auto<br>
6.如何实现点赞转发那里基本样式相同，但首尾个例样式不同：==:not(:last-child)伪类选择器==<br>
7.阴影效果：box-shadow属性<br>
8.怎么画居中的线：将块元素高度设置为1<br>
9.负margin的应用：用负margin移动标题，使蓝条能占用padding的位置，中间的空白用子元素的padding<br>
10.flex适合左右布局<br>
11.列表类结构用ul-li更语义化<br>
12.设置min-width避免首页页面收缩过小导致页面混乱

# 疑问
1.为什么header的p的margin-top和参考页面设置的一样，实际大小却不一样<br>
2.body的lint-height：1是为了什么<br>
3.为什么info类为flex时横线无法显示<br>