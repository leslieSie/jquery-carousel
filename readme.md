#jquery-carousel使用文档
该插件主要要实现的功能是实现一种特色的轮播效果，为网页增强更高的用户体验
####相关的介绍文章
[jquery-carousel的制作思路与分析]()
###插件构成
这款插件主要可以分成两部分<br>
1. 插件初始化<br>
2. API交互

###API说明
1、init(json)
>注：这个方法主要使用来初始化轮播插件的配置，如果传入为空或者不进行传参的话，那么插件将采用默认的配置进行初始化<br>
>JSON格式如下:  
<pre>json:{
	direction    STRING   ['default':'right']
	//这个属性主要是用来设置轮播图的旋转方向，可选的选项为right ,left 默认选中right
	animate:{
		speed:  STRING|INT  ['default':'normal']
		//这个属性用来设置轮播图的
	}
	//这个属性包含轮播动画的一些设置
}</pre>
