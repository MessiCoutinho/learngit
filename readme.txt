搜索
me and my brokenheart

git的常用命令

git init

git add  xx.txt

git commit xx.txt -m"此处填写修改注释"

git status //查看状态

git diff  //查看修改明细

git log  //查看日志

git log --pretty=oneline //查看简明日志

cat xx.txt  //读取文件内容

git reset --hard HEAD^  //退回上个版本、HEAD^^:上上个版本、HEAD~20:前第20个版本

git reflog   //所有的版本id

git reset --hard 1094a  //指定回到未来的某个版本 1094a是版本id的前几位

git diff HEAD -- readme.txt //查看工作区（leangit）与版本库（.git）的区别

git checkout -- readme.txt //让这个文件回到最近一次git commit或git add时的状态

git checkout -b xxx  //创建一个新的分支xxx并切换

git merge xxx  //将分支xxx合并到当前分支

git branch -d xxx  //删除分支分支xxx

cat .git/HEAD  //查看当前分支及路径

git branch  //查看当前分支是哪个

创建分支：git branch <name>

切换分支：git checkout <name>

【配置远程库时遇到的错误】
提示信息为：$ git push -u origin master
fatal: unable to access 'https://github.com/MessiCoutinho/learngit.git/': error setting certificate verify locations:
  CAfile: D:/xxx/Git/mingw64/ssl/certs/ca-bundle.crt
  CApath: none

具体解决办法是： 
使用git 客户端输入一下命令即可：

$ git config --global http.sslverify "false"

git push  /在commit之后，提交到远程仓库

测试我的第二个分支	
Creating a new branch is quick AND simple.
