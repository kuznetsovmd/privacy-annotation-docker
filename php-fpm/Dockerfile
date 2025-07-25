FROM php:8.0-fpm-alpine

RUN apk add libzip-dev
RUN docker-php-ext-install pdo pdo_mysql zip

COPY php.ini /usr/local/etc/php

CMD chown -R www-data:www-data /var/www && php-fpm
