# Docker-for-PHP-projects-with-Apache-and-MySQL

Laying down docker-compose YML file

docker-compose.yml

To set a docker-compose, you need first to select the Compose file versions you want to use, the services you want to provide, and the containers you want to run.
to check Compose file version version: https://docs.docker.com/compose/compose-file/compose-versioning/#compatibility-matrix

In my case i have Docker version 1.13.1 so compose file version is 3.0

version: '3.8'
services:
  php-apache-environment:
    container_name:
    
Setup and run a local PHP Apache server instance

To set up a PHP Apache container, you need to specify the following environments,

The container name
For example container_name: php-apache

The container image
image: php:8.0-apache

The volume - this will set up your present working src directory for your code/source files. If you were to run a PHP script, that file would have to be in that directory.

volumes:
  - ./php/src:/var/www/html/


PHP-login page 

run docker compose file

Docker-compose up -d

cd ./php/src

![image](https://user-images.githubusercontent.com/32263261/154813584-6dfeaef3-60f1-4b68-9ee1-ff3dc72da547.png)

set database in PHPMyAdmin service









    
    
