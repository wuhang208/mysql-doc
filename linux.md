# linux 的简介跟简单命令
## 知识点
  * Linux 历史
  * 人物介绍
  * 简单命令
  
## linux的历史
在1991年，林纳斯·托瓦兹开始在MINIX上开发Linux内核，为MINIX写的软件也可以在Linux内核上使用。后来使用GNU软件代替MINIX的软件，因为使用从GNU系统来的源代码可以自由使用，这对Linux的发展是有益。使用GNU GPL协议的源代码可以被其他项目所使用，只要这些项目使用同样的协议发布。为了让Linux可以在商业上使用，林纳斯·托瓦兹决定更改他原来的协议（这个协议会限制商业使用），以GNU GPL协议来代替。之后许多开发者致力融合GNU元素到Linux中，做出一个有完整功能的、自由的操作系统。

Linux的第一个版本在1991年9月被大学FTP server管理员Ari Lemmke发布在Internet上，最初Torvalds称这个内核的名称为“Freax”，意思是自由（“free”）和奇异（“freak”）的结合字，并且附上“X”这个常用的字母，以配合所谓的类Unix的系统。但是FTP服务器管理员嫌原来的命名“Freax”的名称不好听，把内核的称呼改成“Linux”，当时仅有10000行程序码，仍必须运行于Minix操作系统之上，并且必须使用硬盘开机；随后在10月份第二个版本（0.02版）发布，同时这位芬兰赫尔辛基的大学生在comp.os.minix上发布一则消息

Hello everybody out there using minix- I’m doing a (free) operation system (just a hobby, won’t be big and professional like gnu) for 386(486) AT clones.

1994年3月，Linux1.0版正式发布，Marc Ewing成立Red Hat软件公司，成为最著名的Linux经销商之一。

Unix & Linux历史源流
早期Linux的开机管理程序（boot loader）使用LILO（Linux Loader），早期的LILO存在着一些难以容忍的缺陷，例如无法识别1024柱面以后的硬盘空间，后来的GRUB（GRand Unified Bootloader）克服这些缺点，具有‘动态搜索内核文件’的功能，可以让用户在开机的时候，自行编辑开机设置系统文件，通过ext2或ext3文件系统中加载Linux Kernel（GRUB通过不同的文件系统驱动可以识别几乎所有Linux支持的文件系统，因此可以使用很多文件系统来格式化内核文件所在的扇区，并不局限于ext文件系统）。

Linux的标志和吉祥物是一只名字叫做Tux的企鹅，标志的由来是因为Linus在澳洲时曾被一只动物园里的企鹅咬了一口，便选择企鹅作为Linux的标志。更容易被接受的说法是：企鹅代表南极，而南极又是全世界所共有的一块陆地。这也就代表Linux是所有人的Linux。

## 人物简介

![wating](https://nts.newbieol.com/static/k6/mySQL/class-001/img/ken.png)   
 
 
 
 *Ken Thompson：C语言之父和Unix之父*
 
 ![wating](https://nts.newbieol.com/static/k6/mySQL/class-001/img/dennis.png)
 
 *Dennis Ritchie：C语言之父和Unix之父*
 
 ![wating](https://nts.newbieol.com/static/k6/mySQL/class-001/img/tanenbaum.png)
 
 *Tanenbaum：Minix开发者*
 
 ![wating](https://nts.newbieol.com/static/k6/mySQL/class-001/img/linus.png)
 
 *Linus Torvalds：Linux之父，芬兰赫尔辛基大学*
 
 ## 简单命令
 ### vim的基本使用
  * i：在当前字符的左边插入
  * I：在当前行首插入
  * a：在当前字符的右边插入
  * A：在当前行尾插入
  * o：在当前行下面插入一个新行
  * O：在当前行上面插入一个新
  * h: 向前移动一个字符
  * j: 向上移动一行
  * k: 向下移动一行
  * l: 向后移动一个字符
  * yy: 复制当前一行
  * dd:剪切当前一行
  * p: 粘贴内容到游标之后
  * P: 粘贴内容到游标之前
### 基本的文件操作
### 比如：
1. touch  file
2. cp file file1
3. cp file  /home/linux/file1
4. mv file   file2
5. mv file  /home/linux/
6. ls -al 
7. cat  file
### 基本的目录操作
### 比如：
1. mkdir dir
2. cp dir   dir1  -a
3. cp dir   /home/linux/dir2  -a
4. mv dir  dir2
5. mv dir  /home/linux/
6. rm  dir  -rf
7. ls -d  dir
8. find  ./dir  -name  "filename"
### 文件的归档和压缩
### 比如：
1. gzip  filename
2. bzip2  filename
3. gunzip filename
4. bunzip2  filename
5. tar czvf  file.tar.gz dir
6. tar cjvf  file.tar.bz2 dir
7. tar cJvf  file.tar.xz  dir
8. tar xvf  file.tar.gz
9. tar xvf  file.tar.xz
 
  
