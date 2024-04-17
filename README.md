This is a Bash script that automates the configuration of a fresh Ubuntu Server. - The file was saved in txt format for redundancy reasons ( safety ).

 Write a bash script to automate the installation and configuration of a web server 
 on a fresh Ubuntu 20.04 server. The script should do the following: 
       Install Nginx, PHP, and MySQL server. 
       Configure Nginx to serve a sample PHP application. 
       Secure the server by setting up a firewall for nginx and OpenSSH and configuring SSH access through 
       public key only. 
       Create a user with sudo access and disable root login. 
 
Your script should take the following command line arguments: 
   --domain: the domain name to be used for the SSL certificate and Nginx server name 
   --email: the email address to be used for Let's Encrypt certificate registration 
   --db-user: the username for the MySQL database 
   --db-pass: the password for the MySQL database
   For every argument you can also consider using an abbreviation. (ex. --domain and -d) 
 
Your script should also generate a strong random password for the user with sudo access. 
Your script should output the following information: 
The server's public IP address 
The MySQL root password
The sudo user's username and password 
 
Your script should be idempotent, meaning that it can be run multiple times without causing any issues or errors.
Your script should be able to handle errors that may occur and also implement logging. 
Your script should also include error handling and logging, with appropriate messages for each step of the
installation process. 

You can assume that all the configuration files are in their default location on an Ubuntu server. 
 
You can assume that the server has a fresh installation of Ubuntu 20.04 and has internet access. 

You should not use any third-party tools or services, such as AWS or Docker. 
 
The following packets need to be installed after an update: nginx, php-fpm, php-mysql, mysql-server.  
 
Please also consider configuring nginx. The actual configuration does not matter but show how you would
#modified/remove/add something to a configuration file.

