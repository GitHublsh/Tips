Tips 1

#### Problem : Android Studio项目中.gitignore不生效

#### Solution :

　　有时我们发现添加.gitignore文件后并没有忽略我们想要忽略的文件，解决方法就是清除一下缓存，原因gitignore对已经追踪(track)的文件无效，清除缓存后文件将以未追踪的形式出现.然后再重新添加提交一下,.gitignore文件里的规则就可以起作用了

	git rm -r --cached .
	git add .
	git commit -m 'update .gitignore'

