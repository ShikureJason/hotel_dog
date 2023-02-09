FROM php:8.2.1-fpm-buster

RUN docker-php-ext-install bcmath pdo_mysql
RUN apt-get update
RUN apt-get install -y git zip unzip
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

WORKDIR /var/www

