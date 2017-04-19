FROM php:fpm

RUN apt-get update -y && apt-get upgrade -y

RUN apt-get install libmcrypt-dev libreadline-dev -y

RUN docker-php-ext-install pdo pdo_mysql iconv 

ADD crontab /etc/cron.d/laravel-cron

RUN chmod 0644 /etc/cron.d/laravel-cron