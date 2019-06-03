## web 项目部署到 Ubuntu 中的 tomcat8 

### 1、首先我们现在一个 unzip 解压工具

                1、sudo apt-get install unzip

### 2、通过 SSH 协议传过了的压缩包可以 cp 到：


                1、 cp XXX.war /var/lib/tomcat8/webapps/                        # tomcat8 是 linux 自动的tomcat， 如果是在网上下载的，也一样是放在 webapps 目录下

                2、 service tomcat8 restart                                     # 重启 tomcat 服务， 启动服务进行访问就可了


