INSTALLATION

(This instructions assume that the root will run the commands if you are a user try the commands adding sudo in the beggining of the command)

1.- Verify that you have installed your data server

For mysql 	: apt-get install mysql-server
For postgresql 	: apt-get install postgresql
For sqlite	: apt-get install sqlite3

2.- Run your service

For mysql	: service mysql start
For postgresql	: service postgresql start

Sqlite don't needs to be started

3.- Run the Deb with dpkg

dpkg -i path_to_deb/drupal8_8.2.2-1_all.deb 

4.- Apply apt-get to install dependencies and the package

apt-get install -f

5.- Use the prompts that will be showing to help you configure your database

6.- When the installation ends restart apache

service apache2 restart

7.- In the browser got to to the url of your server adding /drupal8/core/install.php

Ex: localhost/drupal8/core/install.php
