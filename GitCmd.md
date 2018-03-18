# Git常用命令

###	1.初始化仓库
>git init

###	2.提交文件
>git add f1.txt f2.txt 

>git commit -m "备注"

###	3.查看状态
>git status

###	4.详细比对
>git diff

>git diff HEAD -- f1.txt 

###	5.查看记录
>git log

>git log --pretty=oneline

>git reflog

###	6.恢复版本
>git reset --hard HEAD^

>git reset --hard commit_id

###	7.撤销修改
>git checkout -- f1.txt	（从暂存区更新下来工作区,没有则从版本库更新下来）

###	8.撤销暂存区
>git reset HEAD f1.txt	（重置暂存区）

###	9.添加delete到暂存区
>git rm f1.txt

###	10.GitHub添加远程库
>git remote add origin git@github.com:13631372596/Learn_Git.git

>git push -u origin master

>git push origin master

>git push origin dev

### 11.克隆远程库
>git clone origin git@github.com:13631372596/Learn_Git.git

### 12.创建分支
>git checkout -b tree1

>git branch tree2

>git checkout tree2

### 13.查看分支
>git branch

### 14.合并某份之到当前分支
>git merge tree2

>git merge --no-ff -m "no-ff" tree2

### 15.删除分支
>git branch -d tree2

### 16.查看日志记录
>git log --graph --pretty=oneline --abbrev-commit 

>git log --graph

### 17.隐藏工作区及恢复删除
>git stash

>git stash list

>git stash apply

>git stash pop

### 18.查看远程库
>git remote -v

### 19.创建远程库分支到本地并提交
>git checkout -b dev origin/dev

>git push origin dev

### 20.在本地创建和远程分支对应的分支,更新项目
>git branch --set-upstream branch-name origin/branch-name

>git pull

>git fetch origin

>git branch --all

>git merge origin/dev

### 21.创建标签并查看,可指定标签信息
>git tag v1.0

>git tag

>git show v1.0

>git tag -a "v1.1" -m "create v1.1" commit_id

### 22.删除本地标签和远程标签
>git tag -d v1.0

>git push origin :refs/tags/v1.0

### 23.配置Git名字和Email地址,并生成SSH Key
>git config --global user.name "xxx"

>git config --global user.email "xxx@xxx.com"

>cd ~/.ssh

>ssh -keygen -t rsa -C "xxx@xxx.com"

### 24.在工作区定义".gitignore"文件
[点击查看.gitignore](https://github.com/github/gitignore)
	
	# Windows:
	Thumbs.db
	ehthumbs.db
	Desktop.ini

	# Python:
	*.py[cod]
	*.so
	*.egg
	*.egg-info
	dist
	build

	# My configurations:
	db.ini
	deploy_key_rsa

### 25.强制添加文件和查看忽略规则
>git add -f xxx.class

>git check-ignore -v xxx.class

### 26.配置快捷键
>git config --global alias.st status







