# linux笔记

#### 11月12号

源：*/etc/apt/sources.list*

源的下载地址：*https://mirrors.ustc.edu.cn/repogen/（当提示没有release文件等问题可以查看下源是否有更新）*

更新源：*update是下载源里面的metadata的。包括这个bai源有什么包，每个du包什zhi么版本之类的；upgrade是根dao据update命令下载的metadata决定要更新什么包(同时获取每个包的位置)。*

安装vimplug：*装Vundle，然后vim下PlugInstall。*

#### 11月13号

##### conda相关的指令：

*激活：source activate name*

*取消激活： source deactivate*

*创建：conda create -n name python=version*

*打包：conda install* 

*查看：conda list*



/opt目录：*第三方辅助软件放置目录，或是放置在/usr/local下。乱放可能导致权限的问题。*



##### github相关：

git config --global user.name "你的用户名" 

git config --global user.email "你的邮箱"

git config --global core.editor 默认编辑器

ssh key：~/.ssh/id_rsa.pub

创建ssh公钥：ssh-keygen -t rsa -C "你的邮箱"

初始化仓库：git init

设置远程仓：git remote add res_name url  res_name：名字  url远程仓地址

添加文件：git add 目录

提交到本地仓：git commit .

push操作：git push url

