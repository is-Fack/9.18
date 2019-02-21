##Charles(抓包工具) （我的版本 ： 4.1.2）
	( # )代表了 权重 权重高的 实用性强。。。
###开始说明
	Charles正版需要收费 本文附安装破解教程
	https://blog.csdn.net/qq_28831197/article/details/81196571
###工具栏
	首先看工具栏 (以 扫把 开始)
	1.扫把 Clear the current Session （清除所有抓到的包）
	2.录音机 Start recording (开始抓包)
	3.小乌龟 Start Throttling (节流)
		这个就是降低你的浏览器网速 本来一秒打开的 节流开启后
		可能需要10秒
	4.六边形 Enable Breakpoints (启动断点)
		请参照断点调试
	后面的都没用过...(以后再补吧)
###开始使用
	1.首先第一步找到工具栏上方的 proxy 点击 windows Proxy 看到 这个选项左侧 有 √ 号
	  然后点开 录音机 开始抓包  打开你的浏览器 随便上个网址(现在只能抓取http的包 https的包里显示 <unknown> 解决方案参照  证书安装 )
###证书安装
	给你个网址，一步一步来吧
	第一个
	https://www.jianshu.com/p/0c95595e928d
	证书实在安不上 （用这个）
	https://blog.csdn.net/qq_15017407/article/details/53634878
###设置代理
	点击工具栏上方 tools --> Map local... 
	勾选 Enable Map Local
	点击 Add 填写
			例子  https://m.nuomi.com:443/component/nuomi_cashier/3.3.8/order_create/order_create.js
		Protocol (协议)    例:(https)
		Host  填写域名	   例:(m.nuomi.com)
		Port  http 80  https 443  例:(443)
		path  文件名   例:(component/nuomi_cashier/3.3.8/order_create/order_create.js)
		Query (基本不用填)
		Local path  本地的文件
			Case-sensitive 勾√上；
		这样就可以本地文件代理线上文件了。。。
###断点调试
	1.首先找到要打断点的文件 右键 点击 Breakpoints.
		2.点击工具栏 上方的 Proxy --> Breakpoints Settings
		3.找到你设置断点的文件 双击  把 Query 里的全删了 改成 *
		4.Query 下方的两个设置(Request (请求) , Response (返回) ) 根据需要勾选;
		5.刷新页面 ，Charles会自动谈出来跳到(Breakpoints)中
		6.点击 Edit Response --> Text
		7.这就是本次(Request)请求的参数 或是 (Response)返回的数据
		8.可以修改Text里的值 点击 Execute，就修改你想要修改的文件了
		9.下方三个按钮的功能  
			（1）Cancel //取消 
			 (2) Abort //中止
			 (3) Execute //执行
		应该都知道意思，不解释了。
###手机抓包
	没用过...（以后再补）
####设置只关注某些网址
	1.点击工具栏上方的 View --> Focused Hosts
	2.点击 Add 输入想要关注对应的信息 点击 ok;
	3.你会发现 你不想关注的包 都在 Other Hosts里 ，这样是不是感觉好多 (然而并没有什么用)。。。