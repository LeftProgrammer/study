多人协同开发
分为如下几个步骤：
1.创建一个git裸服务器 （git init --bare）

2.从裸服务器将版本库克隆至本地（git clone git版本服务器地址）

3.本地常规操作
git add 文件名
git status 
git commit -m 提交的内容描述

4.推送版本至服务器 （git remote +  git push origin master）
git remote	——知道服务器在哪儿
git push origin master	——将修改内容提交
5.从远程服务器拉取版本（git pull）

分支的使用
分支的基本操作
基本操作有如下几个：

1. 查看当前分支 （git branch）

2. 创建分支 （git branch 分支名）

3.切换分支（git checkout 分支名）

4.分支上的常规操作
使用git add 和git commit提交。
使用git log查看即可

5.分支的合并 （git checkout master + git merge 分支名）
git checkout master
git log
git merge 分支名

6.分支的删除（git branch -d 分支名）



you need to resolve your current index first 解决办法
错误：您需要先解析当前索引
https://blog.csdn.net/jiangyu1013/article/details/78853407
git reset --merge 	——退回merge前


"There is no tracking information for the current branch" 解决方法
当前分支没有跟踪信息。
git branch --set-upstream-to=origin/本地分支


git reset HEAD^就是将HEAD指针前移，指向上一个快照
而已
git log --graph --all	——查看版本状态
git log --graph --pretty=oneline --abbrev-commit 查看整个版本线的状态！
git status看下状态

在master分支上开辟一个新的develop分支，然后我们根据功能或者业务，再在develop
分支上另外开辟其他分支，完成分支上的任务后，再将这个分支合并到develop分支上！
master分支：可直接用于产品发布的代码，就是正式版的代码
develop分支：日常开发用的分支，团队中的人都在这个分支上进行开发
临时性分支：根据特定目的开辟的分支，包括功能(feature)分支，或者预发布(release)分支，
又或者是修复bug（fixbug）分支，临时性分支用完之后一般都会删除，使得代码库的常用分支始终
只有两个长期分支！

