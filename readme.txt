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
rollback for one step
git checkout -- readme.txt
rollback from stage area
git reset HEAD readme.txt
rollback from working area
git checkout -- readme.txt
场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令git checkout -- file。
场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令git reset HEAD file，就回到了场景1，第二步按场景1操作。
场景3：已经提交了不合适的修改到版本库时，想要撤销本次提交，参考版本回退一节，不过前提是没有推送到远程库。
rm delTest.txt
git status
Delete it persistently
git rm delTest.txt
git commit
Rollback from delete
git checkout -- delTest.txt
register a SSH code
ssh-keygen -t rsa -C "yangsheng_net@hotmail"
$ ssh-keygen -t rsa -C "yangsheng_net@hotmail"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/yangshen/.ssh/id_rsa):
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/yangshen/.ssh/id_rsa.
Your public key has been saved in /c/Users/yangshen/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:WP0FTRszjIpKP5cJkM+z73id6XwjzSAiqd3dxn8yAM8 yangsheng_net@hotmail
The key's randomart image is:
+---[RSA 2048]----+
|       .    .==  |
|      o  .  ..o= |
|       +....  o  |
|      .o* o. .   |
|     ..+S+ *.    |
|      + = = E    |
|     o o * = B   |
|    . . ..+.O B .|
|        .o.oo+.= |
+----[SHA256]-----+
$ ssh-keygen -t rsa -C "yangsheng_net@hotmail.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/yangshen/.ssh/id_rsa):
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/yangshen/.ssh/id_rsa.
Your public key has been saved in /c/Users/yangshen/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:zsqgAK4LpDL8onDfATOgAvla43s/iDnigQ0j3279hqY yangsheng_net@hotmail.com
The key's randomart image is:
+---[RSA 2048]----+
|                 |
| .               |
|o .              |
|.o .             |
|B.+ +   S        |
|XO o + o         |
|X+=ooo..o        |
|*=*=++=o.        |
|*++=E+=+.        |
+----[SHA256]-----+
C:\Users\yangshen\.ssh
GitHub https://github.com/
git config --global http.proxy http://userName:password(encoded)@proxyaddress:port
git config --global http.proxy http://web-proxy.corp.hp.com:8080
echo # SPHugeLinkField >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/yangshengnet/SPHugeLinkField.git
git push -u origin master
$ git push -u origin master
Counting objects: 28, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (23/23), done.
Writing objects: 100% (28/28), 72.93 KiB | 0 bytes/s, done.
Total 28 (delta 6), reused 0 (delta 0)
To https://github.com/yangshengnet/SPHugeLinkField.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.
Store your credentials locally
$ git help credentials
$ git config credential.helper store
$ git push https://github.com/yangshengnet/SPHugeLinkField.git
Username: <type your username>
Password: <type your password>

