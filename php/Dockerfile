FROM php:fpm
COPY ./php.ini /usr/local/etc/php/conf.d/
RUN apt-get update \
  && apt-get install -y libfreetype6-dev libjpeg62-turbo-dev libpng12-dev libmcrypt-dev libssl-dev \
  && docker-php-ext-install pdo_mysql mysqli mbstring gd iconv mcrypt json ftp zip
