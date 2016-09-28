#jquery-carousel使用文档
该插件主要要实现的功能是实现一种特色的轮播效果，为网页增强更高的用户体验
####相关的介绍文章
[jquery-carousel的制作思路与分析]()
###插件构成
这款插件主要可以分成两部分<br>
1. 插件初始化<br>
2. API交互(1.0版本暂未开通)

###API说明
1、init(json)
>注：这个方法主要使用来初始化轮播插件的配置，如果传入为空或者不进行传参的话，那么插件将采用默认的配置进行初始化<br>
>初始化JSON格式如下:  
<pre>json:{
	//边框是否有阴影
	showdow   INT    ['default',0]
	//定义图片与图片之间的空隙
	interval   percent|px   ['default','5%']
	//定义图片的宽度
	width     percent|px    ['default','15%']
	//这个属性包含轮播动画的一些设置  
	animate:{
		direction    STRING   ['default':'right']
		//这个字段主要是用来设置轮播图的旋转方向，可选的选项为right ,left 默认选中right
		speed  STRING|INT  ['default':'normal']
		//这个字段用来设置轮播图轮播的速度，也即是过度时间，目前支持slow,normal,fast三种模式
		stayTime   INT   ['default':800]
		//这个字段用来描述图片停留展示的时间，单位为ms
		isDelay    BOOL  ['default':false]
		//这个字段是用来判断加载后轮播图是否延迟动作,默认为false,也就是不开启
		delay	   INT   ['default',0]
		//标识延迟的时间，只有在isDelay设置为true的时候才生效
			}
	//这个属性是用来添加轮播图的缩略图，圆形等视图工具
	tool:{
		status    BOOL    ['default':false]
		//这个字段是用来检测附属工具是否开启，默认为false为不开启
		type      STRING  ['default','circle']
		//这个字段是设置附属工具的类型的，目前支持circle圆形显示,overviewImg缩略图显示
		}
	}
</pre>
###DEMO