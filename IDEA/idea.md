### 在Linux/Ubuntu中快速安装IDEA
- 一般的在安装第三软件时，Linux是不会在系统中有IDEA这样的商业软件的，所以借助两个命令来安装第三方软件
   
### wget使用
- wget url(这里url就是你要下载idea的网站)
- [在idea官网中direct link右键复制链接](1.jpg)
- [wget下载](1.png)

### 如果觉得wget下载太慢，可以执行停止（按Ctrl + C）是用axel命令
- 首先要在终端查找看一下是已经下载了
		apt search axel 命令
		如果没有下载可以使用命令下载: sudo apt install axel
- 下载axel命令后
		axel -n 32 url 		(32个线程下载)
 		-n:表示启动线程，启动多少看后面带的参数
	

### 我们要进行解压
- tar&nbsp;&nbsp;xvzf&nbsp;&nbsp;  文件名.tar.gz
- 解压完后要切换bin目录下
- 执行&nbsp;./idea.sh&nbsp;命令，idea就会进行安装了
