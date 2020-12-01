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
tar -zxvf apache-maven-3.6.3-bin.tar.gz
git config --global user.email "你的邮箱"

git config --global core.editor 默认编辑器

ssh key：~/.ssh/id_rsa.pub

创建ssh公钥：ssh-keygen -t rsa -C "你的邮箱"

初始化仓库：git init

设置远程仓：git remote add res_name url  res_name：名字  url远程仓地址

添加文件：git add 目录

提交到本地仓：git commit .

push操作：git push url

#### 11月20号
b：设备文件。

c：串行端口设备。

s：套接字。


##### 用户权限

[user group other]

drwxr-xr-x. 13 root root   155 Nov 16 04:22 

13：与他相关的资源数

两个root：拥有者和所属群组

155：大小

后面的是修改时间。

Nov 16 04:22 ：格式  date-time

单点登录：一次登录，在其余设备就不需要登录了。

更换组及用户：chown -R silver:testgroup ./test

联级更改权限的参数都是-R。

权限 ： 

s，该文件可执行，执行后该用户进入其文件所属组。

t：

#### 11月23日
usermod ： usermod -a -G testgroup silver
linux配置java：环境变量配置在/etc/profi    ~/.bashrcle,但是这是全局环境变量，如果h配置在个人环境下就是    ~/.bashrc

tar -cvf 目标文件 源路径   ：将源路径下的所有东西打包到目标文件
   >c：建立tar包或者压缩包
    输入密码
tar -zxvf 目标   ：将目标解压
   >z：是否同时用gzip压缩.
   
   >x：解压或者解包
   
   >v：可视化
    
   >f：后面跟文件名（只能写在最后面）

shell script：

>unset：取消变量

>readonly:变量只读

>‘’作为变量内容时，里面所有东西全是字符串。

#### 11.24

echo ${#name} 加#可以得到长度

echo ${name:1:3} 字符串切片

echo `expr index "hellow" b  找字符，先找到谁就返回其

数组：

> arrs=(v0 v1 v2 v3 v456)

> echo ${arrs[2]}

http://packages.deepin.com/deepin/pool/non-free/d/deepin.com.qq.im/

