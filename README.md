# Docker-PHP
Simple Php7.4/Composer/phpunit env launched with docker


# Initialize

* git clone git@github.com:Loic-Hakisa/Docker-PHP.git
* cd Docker-PHP
* docker-compose run composer install


# Launch units tests from "tests" folder:

* docker-compose run phpunit


# Start PHP Fpm container and use files from local /src folder in container /var/www/html/

* docker-compose up -d fpm
* php info.php
* docker-compose down

