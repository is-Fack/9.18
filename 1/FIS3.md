##类似webpack的前段构件化工具
    FIS3不会修改源码，只能通过设置将结果输出到指定目录中。
###核心
	资源定位、内容嵌入、依赖声明
###使用方法
	发布
	//发布到 fis3内置的服务器上
	fis3 release 
	启动
	fis3 server start
	修改端口
	fis3 server -h
	文件监听
	fis3 release -w
	浏览器自动刷新
	fis3 release -wL
