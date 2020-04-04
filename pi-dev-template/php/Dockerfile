ARG PHP_VERSION
FROM php:$PHP_VERSION
RUN apt-get update;\apt-get upgrade;\docker-php-ext-install mysqli
COPY php.ini /usr/local/etc/php/