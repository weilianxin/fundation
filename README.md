# README

记录前端学习内容

gitbook初使用

下载git
安装后创建和github仓库同名的文件夹当本地库
然后在刚创建的文件夹中右键，点击git bush here

第一步
git init 进行初始化，会生成一个.git文件
如果不小心在错误的文件夹中进行了git init，只要把.git文件删除，这就相当于删除了git本地库

第二步
git checkout -b master
创建本地master分支，并切换到该分支

第三步
git remote add origin <https://github.com/weilianxin/fundation.git>
添加远程库（但这时还没有绑定远程库的分支）

第四步
git pull origin master
拉取远程库master分支的内容到本地当前操作的（master）分支

第五步
git config --global user.name "weilianxin"
git config --global user.email "792665319@qq.com"
创建账号和邮箱

第六步
写代码，然后git add .
然后 git commit -m "first"

第七步
git push origin master 推送到远程库
这时会让你认证一下个人信息，github进行授权
授权完成就大功告成了

git 部分命令解释
git init 将文件夹初始化成git环境，即生成.git文件夹
git add . 添加文件到本地暂存区
git commit -m "first" 提交文件到本地库
git status 查看本地库和暂存区的内容
git branch 查看所有分支以及当前分支，当前分支前会加*变绿
git branch branchName 生成一个新的，名叫branchName的分支
git checkout branchName 切换到名叫branchName的分支，如果没有该分支，则创建该分支并切换到该分支
git checkout -b branchName 创建并切换到叫branchName的分支
git remote -v 查看所有分支
git remote add 远程库名 远程库地址 （相当于链接本地库和远程库）
git clone git://github.com/jquery/jquery.git 不用当前文件夹是git环境，直接拉下来代码

git push origin master 将当前操作的本地库分支推送到远程库master分支
git push origin wlx:master 将本地的wlx分支推送到远程master分支
注意，如果wlx没有，直接git push origin :master 相当于推送一个空库到远程，就相当于产出远程分支

git pull origin master 拉取远程库master分支到本地当前操作分支
git pull origin master:brantest 拉取远程库master分支合并到brantest分支

gitbook，github，git，vscode三者联合记笔记
