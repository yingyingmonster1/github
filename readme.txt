git add <filename> --添加文件
git commit -m "change message"  --提交
git status  --查看状态
git diff --查看修改内容
git reset --hard HEAD^  --回退到上一版本
git reset --hard <版本号>  --回到该版本
git reflog --查看之前的命令
git checkout --<filename>  --把该文件恢复成最新版本
git reset HEAD <filename>  --把暂存区的修改撤销掉，重新放回工作区
git rm <filename>  --在版本库中删除文件（之后要进行commit）
git remote add origin git@github.com:<gitnanme>/<projectname>.git  --关联远程库
git push -u origin master  --把本地内容推送到远程库并整合分支
git push origin master  --把本地master分支推送到github
git clone <website>  --克隆远程库
git checkout -b <branchname>  --创建并切换分支
	=git branch dev
	 git checkout dev
git branch -d <branchname>  --删除远程库
git merge <branchname>  --合并分支（删除非主分支）
git merge --no-ff -m "message" <branchname>  --合并企且保留分支
git stash  --把当前的工作存起来，等恢复后继续
git stash list  --查看存起来的工作区
git stash apply  --恢复存起来的工作区  git stash drop  --删除存起来的工作区
	=git stash pop
git cherry-pick <commit id>  --把特定的提交合并到当前分支
git branch -D <branchname>  --强行删除当前分支
git remote  --查看远程库信息
git remote -v  --查看相信的远程库信息
git checkout -b <branchname> origin/<branchname>  --克隆远程分支到本地
git pull  --抓取最新分支
git branch --set-upstream-to=origin/<branchname>  <branchname>  --设置本地分支与远程分支链接
git rebase  --把分支变成一条线
git tag <tagname>  --给当前的分支的最新提交打标签
git tag <tagname> <commit id>  --给对应的提交打标签
git tag  --查看打的标签
git show <tagname>  --查看打的标签
git tag -a <tagname> -m "tag message" <commit id>
git tag -d <tagname>  --删除本地标签
git push origin :refs/tags/<tagname>  --删除远程标签
git push origin <tagname>  --将某个标签推送到远程
git push origin --tags  --将所有标签推送到远程