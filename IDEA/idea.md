### 一、在L inux/Ubuntu中快速安装IDEA

- 在安装第三软件时，Linux是不会在系统中有IDEA这样的商业软件的，所以借助wget、 aexl两个命令来安装第三方软件
   
### 二、wget使用
-  wget url(https://download.jetbrains.com/idea/ideaIU-2018.3.5.tar.gz)
- ![在idea官网中direct link右键复制链接](img/1.jpg)  
- ![wget下载](img/1.png)


### 三、如果觉得wget下载太慢，可以执行停止（按Ctrl + C）是用axel命令
- 首先要在终端查找看一下是否已经下载axel
		apt search axel 命令
		
		如果没有下载可以使用命令下载: sudo apt install axel
		
- 下载axel命令
		axel -n 32 url 		(32个线程下载)
 		-n:表示启动线程，启动多少看后面带的参数
	

### 四、要对文件进行解压
- 解压文件

		tar xvzf  文件名.tar.gz
		
- 解压完后要切换bin目录
  
	   cd 文件名/bin
	  
- 执行命令，idea就会进行安装了

		./idea.sh


### 五、配置文件迁移

	 whereis tomcat8  -- 查询位置
	 
	 sudo ln -s /etc/tomcat8 /conf
