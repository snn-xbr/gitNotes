git config --global user.name 'XXXX'
git config --global user.email 'XXX'
初始化git仓库
cd D:
mkdir gitNotes
touch readme.txt
git init
ls -a
提交文件
git status
git add readme.txt
git commit -m 第一次提交
git log --pretty=oneline
分支管理
git checkout -b dev
cat readme.txt
vim readme.txt
git add readme.txt
git commit -m dev上的提交
git checkout master
git merge master
git branch -d dev
