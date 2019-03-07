### 一、什么是ftp协议
- ftp是文件传输协议，是TCP/IP协议组中的协议之一，它分成两个部分，一个是ftp服务器，另一个是ftp客户端；主要存储文件的。
- 缺点：ftp协议传输文件，在传输过程中，往往会暴露文件里面的信息内容。
### 二、什么是ssh协议
- ssh是一种加密的网络传输协议，可在不安全的网络中为服务提供安全的传输环境。
- ssh通过在网络中简历安全隧道来实现ssh客户端与服务器之间的连接。

### 三、Linux/Ubuntu安装和启动ssh
- 首先要先查看系统是否有ssh:  apt search ssh
- 其次没有就要去下载ssh: sudo apt install openssh-server
- 然后要去修改sshd_config文件
- [sshd_config](1.png)
- 最后，在Windows或Linux其他终端执行scp命令就可了
- [scp](2.png)

### 四、上传本地文件到远程机器指定目录
- scp /opt/test.tar 用户名@IP地址:/home/用户名

### 五、上传本地目录到远程机器指定目录
- scp -r /opt/test 用户名@IP地址:/home/用户名

### 六、从远程复制到本地
- scp 用户名@IP地址:/opt/test/test.tar 本地路径

### 七、从远程复制文件到本地目录
- scp -r 用户名@IP地址:/opt/test 本地路径
