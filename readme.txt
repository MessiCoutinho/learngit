搜索
me and my brokenheart

测试回退

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