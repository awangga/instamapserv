#Web Server Instalation.

# Introduction #

Red Hat Enterprise Linux 6 x86\_64 Instalation :
  1. Apache
  1. Mysql
  1. PHP
  1. phpMyadmin

Reference
  * [How To Forge](http://www.howtoforge.com/quick-n-easy-lamp-server-centos-rhel)
  * [Tecadmin](http://tecadmin.net/installing-apache-mysql-php-on-centos-redhat/#)
  * [Unixmen](http://www.unixmen.com/install-lamp-server-in-centos-6-4-rhel-6-4/)
  * [Redhat](http://www.redhat.com/magazine/003jan05/features/lamp/)
  * [AArif blog](http://linuxaarif.blogspot.com/2013/02/lamp-or-apache-server-installtion-in.html)
# Details #

```
#!/bin/bash
yum install httpd -y
service httpd start
chkconfig httpd on


yum install mysql mysql-server -y
service mysqld start
chkconfig mysqld on

mysql_secure_installation

yum install php -y
yum install php-mysql -y



#Install phpMyAdmin

wget ftp://ftp.sunet.se/pub/Linux/distributions/scientific/6.3/x86_64/updates/security/php-mbstring-5.3.3-27.el6_5.x86_64.rpm
rpm -ivh php-mbstring-5.3.3-27.el6_5.x86_64.rpm
wget http://mirror.smartmedia.net.id/epel/6/x86_64/libmcrypt-2.5.8-9.el6.x86_64.rpm
rpm -ivh libmcrypt-2.5.8-9.el6.x86_64.rpm
wget http://mirror.smartmedia.net.id/epel/6/x86_64/php-mcrypt-5.3.3-3.el6.x86_64.rpm
rpm -ivh php-mcrypt-5.3.3-3.el6.x86_64.rpm
wget http://mirror.smartmedia.net.id/epel/6/x86_64/php-php-gettext-1.0.11-3.el6.noarch.rpm
rpm -ivh php-php-gettext-1.0.11-3.el6.noarch.rpm
wget http://mirror.smartmedia.net.id/epel/6/x86_64/phpMyAdmin-3.5.8.2-1.el6.noarch.rpm
rpm -ivh phpMyAdmin-3.5.8.2-1.el6.noarch.rpm
#config file vi /etc/httpd/conf.d/phpMyAdmin.conf
service httpd restart

```

Open Firewall by editing iptables :
```
iptables -A INPUT -m state --state NEW -m tcp -p tcp --dport 80 -j ACCEPT
```
save iptables:
```
iptables save
```
check iptables:
```
iptables -L -n
```

Securing Apache :
```
http://www.tecmint.com/apache-security-tips/
```