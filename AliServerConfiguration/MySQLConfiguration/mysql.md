## mysql 配置

### 1、要到 **/etc/mysql/mysql.conf.d** 目录下

		1、cp mysqld.conf  /etc/mysql/mysql.cnf			# 把mysqld 中配置复制一份到 mysql.cnf 配置中

### 2、 mysql.cnf 配置

		[mysqld]	
			
			character-set-server = utf8
	
		[mysql]
	
			default-character-set = utf8
		
		[mysql.server]

			default-character-set = utf8

		[client]

			default-character-set = utf8


		
