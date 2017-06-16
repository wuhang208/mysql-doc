# git基础知识
## git简介
## git基本命令
## git分支
## git远程仓库

## gir简介
### 关于GIT
    GIT 是一个分布式版本控制软件，最初由林纳斯·托瓦兹（Linus Torvalds）创作，于2005年以GPL发布。最初目的是为更好地管理Linux内核开发而设计。是目前世界上最先进的分布式版本控制系统.
    
### 安装GIT
1. $ git
2. The program 'git' is currently not installed. You can install it by typing:

*使用下面的命令进行安装git工具.*
1. $ sudo apt-get install git
### 创建版本库
第一步, 先要创建一个目录, 这个目录就是用来存放仓库的.

1. $ mkdir html
2. $ cd html

第二步, 使用git init命令, 将当前目录创建成git仓库.

1. $ git init
2. Initialized empty Git repository in /home/user/html/.git/  

马上就把仓库创建成功了, 并提示这是一个空仓库.

1. $ ls -al
2. .git

### 增加文件
*当前目录里没有文件, 那么我们先创建一个文件README*

 1. touch README

*编辑这个文件, 写一点东西在里面*

2. vim README

*先用查看当前状态的命令, 查看一下现在目录下文件的状态*

3. git status

*把文件加到仓库中去, 只有加到仓库中了, 才可能看一下文件的变化*

 4. git add README

*现在使用查看状态的命令, 看一下是目录下文件的状态*

5. git status
### 提交

1. git commit
### 配置用户信息
1. $ git config --global user.name
2. $ git config --global user.email
### 查看提交信息
1. $ git log

## GIT基本命令
### 删除文件恢复
 只要将文件提交到仓库中，则可以执行以下操作：
 
 若使用rm命令删除文件后 则使用命令 git checkout +文件名 则可以恢复文件
 ### 版本回退
 如果想回退到上次提交的版本, 那么需要使用git reset命令.
  git reset --hard commitID 
  
  要想知道COMMITID，则必须要使用命令 git reflog 
  
 ### 从仓库中删除文件
    想要删除仓库中的文件，需要使用git rm filename
    
    但这还不是真正的从仓库中删除，我们还要将删除操作再一次提交到仓库。
    
    git commit
 ### 从版本中忽略文件
    touch .gitignore
 ### 版本之间的对比
  1. git diff
  2. git diff commitID1 commitID2
 ###  patch
  ##### git生成patch
  git format-patch -p1
  ##### git生成patch
  git am patch-name
## GIT分支
![wating](https://nts.newbieol.com/static/k6/02.git-github-markdown/class-003/images/workflow.png)
## GIT远程仓库
### 添加远程仓库
如果我们现在本地有一个git仓库, 我们使用remote add 命令将它添加到远程的仓库中.

$ git remote add origin https://github.com/wangleihd/h5class.git

并需要将远程的仓库的信息更步到本地, 这里主要指的示远程仓库的分支和远程库的提交变更信息.

$ git fetch origin
### 同步master分支
 git push origin master
### 同步其他分支
 git push origin branch-name
### 同步标签
 git push origin --tags
### 删除远程分支
 git push -u origin :branch-name
### 删除远程标签
 git push origin --delete <branchName>
 git push origin --delete tag <tagname>
### 从远程仓库同步
 #### clone
 git clone url
 #### pull
 git pull
### 命令和状态
![wating](https://nts.newbieol.com/static/k6/02.git-github-markdown/class-004/images/git-status.png)
