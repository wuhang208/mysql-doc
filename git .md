# git基础知识
## git简介
## git基本命令
## git分支
## git远程仓库
## MarkDown基本语法
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
