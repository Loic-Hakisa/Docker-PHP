# Docker-PHP
Simple Php7.4/Composer/phpunit env launched with docker


## Initialize

* git clone git@github.com:Loic-Hakisa/Docker-PHP.git
* cd Docker-PHP
* docker-compose run composer install


## Launch units tests from "tests" folder:

* docker-compose run phpunit


## Start and use PHP-FPM container

Files from local git /src folder are available in container's /var/www/html/ folder.

* docker-compose up -d fpm
* docker-compose exec fpm bash
* php info.php
* docker-compose down

