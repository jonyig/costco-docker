FROM php:7.2-fpm

RUN apt-get update \
 && apt-get install -y --no-install-recommends apt-utils \
 && apt-get install --yes zip unzip \
 && apt-get install -y git \
 && docker-php-ext-install pdo_mysql \
 && curl -sS https://getcomposer.org/installer | php \
 && mv composer.phar /usr/local/bin/composer \
 && ln -s /usr/share/nginx/html/artisan . \
 && ln -s /usr/share/nginx/html .
