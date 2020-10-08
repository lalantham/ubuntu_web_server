![Repo Image](https://github.com/lalantham/ubuntu_web_server/blob/main/ubuntu-apache.jpg)
# Ubutnu Web Server

>Ubuntu Web Server

## 01 - Install Lampp Stack

	1.1 - Install tasksel

	1.2 - tasksel install lamp-server  

## 01 - Config MYSQL
	2.1 - mysql_secure_installation
	
	2.2 - CREATE USER 'newuser'@'localhost' IDENTIFIED BY 'password';
	
	2.3 - GRANT ALL PRIVILEGES ON * . * TO 'newuser'@'localhost';
	
	2.4 - FLUSH PRIVILEGES;
	
	2.5 - create database {Database Name Here}

## 03 - Get Wordpress

	3.1 - wget https://wordpress.org/latest.tar.gz

	3.2 - Extract and Put Files into web root directory
  
 ## 04 - Config wp-config File

	4.1 - Add database details ( database name, database user, password )

	4.2 - Change Salts
  
  	4.3 - Save as wp-config

 ## 05 - Setting up Let's Encrypt

	5.1 - sudo apt install python-certbot-apache
  
  	5.2 - sudo certbot --apache -d example.com

## Related to Oracle Cloud VM Instanses
	
	* sudo iptables -I INPUT 6 -m state --state NEW -p tcp --dport 80 -j ACCEPT
	* sudo netfilter-persistent save
	* sudo systemctl restart apache2
