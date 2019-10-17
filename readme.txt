This is a new start of my life.
Never too late to study.


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
git swich -c <branchname>  --切换到新的git分支
git swich <branchname>  --切换到已有分支
