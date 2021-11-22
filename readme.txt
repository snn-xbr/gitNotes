1.基本配置
git config --global user.name 'XXXX'
git config --global user.email 'XXX'

2.初始化git仓库
cd D:
mkdir gitNotes
touch readme.txt
git init
ls -a

3.提交文件
git status
git add readme.txt
git commit -m 第一次提交
git log --pretty=oneline

4.撤销修改
（1）修改工作区的修改
（2）撤销暂存区的修改（git add的文件撤销方法）
git reset HEAD 文件名 从暂存区中移除文件
（3）撤销已经commit的文件
git reset --hard HEAD^ 使用版本撤销命令,回退到上一个版本

5.分支管理
git checkout -b dev
cat readme.txt
vim readme.txt
git add readme.txt
git commit -m dev上的提交
git checkout master
git merge master
git branch -d dev

6.克隆远程代码
git clone url 文件夹名
