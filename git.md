# git 使用
1. git init
	- 文件夹初始化为git仓库
2. git status 
        - No commits yet  Untracked files;[not added, new files]      
        - No commits yet  Changes to be commited[added] 
        - No commits yet  Changes to be commited[added]  &  Changeds not staged for commit[not added, changed files]
	
3. git diff : 查看区别git add 前后
4. git reset : 把add后的文件 取消add
5. git config --global user.name 'David Chen' push后知道作者名字
6. .gitignore
	- 可以添加到这个文件，如果不想让git帮你管理
7. 上述方式无法 忽略那些已经被tracked 的文件
8. git rm --cached [filename]
	- 这个方法可以解决上述的问题
9. git 分支
	- git branch [branch name]   :  create a branch	
	- git checkout [branch name] :	switch to branch
	- git add 
	- git commit 
	- git checkout master: switch to master branch
	- git merge [branch name] : merge [branch name] to master branch
	- 但是还是保留老的分支
	- git branch: 查看所有分支
	- git branch -d [branch name] : delete branch
	- git branch -D [branch name] : force delete branch
10. github 上创建一个 repo:远程仓库, 然后让本地仓库和远程仓库绑定： 
 	- git remote add origin https://github.com/....git : connected to remote repo;
11. 本地仓库与远程仓库解绑
	- git remote -v : 查看当前本地repo的远程仓库关联情况
	- git remote rm [origin] : 与远程origin解绑
12. git config credential.helper store   : commands before push to save user name and password locally;
13. git push --set-upstream origin master
14. 邀请别的github账户 加入你的项目: 即对该远程repo拥有push的权限
	- github中collaborators 中搜索用户名
15. 合作者流程：
	- git clone https://github.com/..... : 从远处仓库中clone到本地
	- git add .
	- git commit -m '' 
	- git push : 直接push 
	    git config credential.helper store   : commands before push to save user name and password locally;
16. 项目主 把合作者提交的最新修改拉到本地
        - git pull : 把最新修改都拉到本地
 
 
 
