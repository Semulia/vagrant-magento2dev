# Vagrant for Magento 2 developing
This vagrant box with environment optimized for Magento 2 developing.
Including:
 - Debian Jessie 8.6 x64
 - Puppet 3.7.2
 - Percona 5.7.19-17
 - Apache 2.4.20
 - module HTTP/2
 - PHP 7.0.11
 - Xdebug 2.4.1
 - Composer 1.2.1
 - Adminer 4.2.5
 - NodeJS 6.6.0
 - NPM 3.10.8
 - Grunt 1.2.0
 - Gulp 3.9.1
 
 ## HOW TO USE
 Change configs in _vagrant/config.yaml_ file:
 - hostname
 - private_ip
 
 Type next commands in vagrant/ directory:
 - `vagrant plugin install vagrant-hostmanager` (if didn't installed)
 - `vagrant up`
 
 ## Vagrant machine configurations
 You can configurate you machine in _config.yaml_ file.
 
 Allowed configs:
  - **hostname**
  
  set here your project host name, so you will can use http://vagrant.sample instead *private_ip* to access website
  for using this need to install host manager plugin for vagrant - `vagrant plugin install vagrant-hostmanager`
  - **private_ip**
  
  IP address of you project website, you will access to website by this IP address in browser 
  - **use_nfs**
  
  0/1 values, will use or not network file system, strongly reccomend to enable for better permormance
  
  ## Directories
  
  Your project will locate in html directory. On vagrant machine projet locate in /var/www/html/ directory.
  
  Syncing directories ../html -> /var/www/html
  
  ## How to login into vargant machine:
  First way - using vagrant command
  
  `vagrant ssh`
  
  Second way - login through ssh
  
  `ssh vagrant@127.0.0.1`
 
 ## Credentials
  
 ### SSH
 
 username - **vagrant**
 
 password - **vagrant**
 
 
 ### MySQL

 username - **root**
 
 password - **root**
