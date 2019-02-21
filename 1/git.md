###
	切换分支
	远程分支
	git checkout -b 分支 origin/分支
	本地分支	
	git checkout 分支
	查看所有分支
	git branch
	git branch -r （远程分支）
	git branch -a （所有分支）
	删除分支
	git branch -d 分支 （删除本地分支）
	（删除远程分支）
	git branch --delete feacher
	git branch --delete origin feacher 
	查看历史版本
	git log // 查看历史
	git log --decorate --graph --oneline --all // 查看版本以及指向
	拉取代码
	git fetch (获取远程仓库的最新数据)
	git merge origin/master (改变 HEAD,marster 的指针)
	git pull
	提交代码流程
	git add .
	git commit -m '注释'
	git pull
	git push 后
	会报错
	报错里有个代码
	提交那个
	大概是
	git push origin HEAD:路径

	???
	git stash
	git stash pop



	vim 文件名（可以编辑文件）