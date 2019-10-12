######
# See: https://hub.docker.com/_/php/
######

FROM php:7.2.18-fpm
RUN apt-get update && apt-get install -y \
        libfreetype6-dev \
        libjpeg62-turbo-dev \
        libpng-dev \
		libzip-dev \
	&& mkdir -p /var/log/supervisor \
    && docker-php-ext-install -j$(nproc) iconv \
    && docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ \
    && docker-php-ext-install -j$(nproc) gd \
    && pecl install redis \
    && docker-php-ext-enable redis \
	&& pecl install swoole \
    #&& docker-php-ext-enable swoole\
    && pecl install xdebug \
    #&& docker-php-ext-enable xdebug \
    && docker-php-ext-install exif \
    && docker-php-ext-enable exif \
    && docker-php-ext-install pdo_mysql \
    && docker-php-ext-enable pdo_mysql \
	&& docker-php-ext-install bcmath \