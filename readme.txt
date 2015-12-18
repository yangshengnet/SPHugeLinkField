Git download https://git-for-windows.github.io/
user name
$ git config --global user.name "Andy Yang"
user email
$ git config --global user.email "yangsheng_net@hotmail.com"
$ mkdir SPHugeLinkField
$ cd SPHugeLinkField
$ pwd
/c/Users/yangshen/SPHugeLinkField
$ git init
Initialized empty Git repository in C:/Users/yangshen/SPHugeLinkField/.git/
npp download https://notepad-plus-plus.org/download/v6.8.8.html
two steps to add a elephone to refigrator
git add readme.txt
git commit -m "readme Initialized!"
status
git status
difference
git diff
rollback to one step before
git reset --hard HEAD^
rollback to 100 steps before
git reset --hard HEAD~100
rollback according to commit ID
git reset --hard 479db20c4d6c263fbe6e0fa3f5a682668b6a36d7
list commit log
git reflog
LICENSE
check the files between server and client
git diff HEAD -- readme.txt

git checkout -- readme.txt