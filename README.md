The purpose of this project is to set up a LAMP stack
The commands used for intalling Apache, Mysql and php packages can be found below
LAMP is an acronym for Linux, Apache, Mysql and PHP
Together, Linux, Apache, MySQL, and PHP form a popular software stack for building and deploying web applications.

Steps used are stated below
1. I launched an EC2 Instance with Ubuntu Linux OS
2.  I established an SSH connection to the instance using
     ssh -i "key.pem" user@hostname
3.  I installed the components

The commands used for installation can be found below
# Update package lists
sudo apt update

# Install Apache
sudo apt install apache2

# Install MySQL (or MariaDB)
sudo apt install mysql-server

# Install PHP and necessary modules
sudo apt install php libapache2-mod-php php-mysql

4. I startred the respective services on the server

The commands used for starting the services can be found below
# Start Apache
sudo systemctl start apache2

# Start MySQL
sudo systemctl start mysql

5. I ensured the services were running
   
The commands used to ensure services were running can be found below
# Check Apache status
sudo systemctl status apache2    

# Check MySQL status
sudo systemctl status mysql

6. I created a PHP file and tried to connect from a browser on my local machine
This was used to create the php file
<?php
// PHP Info File
phpinfo();
?>


