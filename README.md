![Repo Image](https://github.com/lalantham/ubuntu_web_server/blob/main/ubuntu-apache.jpg)
# Ubutnu Web Server

>Ubuntu Web Server

## 01 - Install Lampp Stack

	1.1 - Install tasksel

	1.2 - tasksel install lamp-server  

## 01 - Config MYSQL
	2.1 - mysql_secure_installation
	
	2.2 - Check git Status --> git status --> | Short Status --> git status -s
	
	2.3 - GRANT ALL PRIVILEGES ON *.* TO {Usrrname Here}@localhost IDENTIFIED BY '{Password Here}';
	
	2.4 - GRANT ALL PRIVILEGES ON * . * TO '{Username Here}'@'localhost';
	
	2.5 - Commiting Without Staging --> gitcommit -a -m "Message Here"
	
	2.6 - FLUSH PRIVILEGES;
	
	2.7 - create database {Database Name Here}

## 03 - Get Wordpress

	3.1 - wget https://wordpress.org/latest.tar.gz

	3.2 - Extract and Put Files into web root directory
  
 ## 04 - Get Wordpress

	4.1 - Add database details ( database name, database user, password )

	4.2 - Change Salts
  
  4.3 - Save as wp-config
