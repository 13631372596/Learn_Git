#Git命令

###	1.初始化仓库
>git init


###	2.提交文件
>git add f1.txt f2.txt 

>git commit -m "备注"

###	3.查看状态
>git status


###	4.详细比对
>git diff


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

### 11.克隆远程库
>git clone origin git@github.com:13631372596/Learn_Git.git

### 12.创建分支
>git checkout -b tree1

>git branch tree2

>git checkout tree2

### 13.查看分支
>git branch

### 14.删除分支
>git branch -d tree2



