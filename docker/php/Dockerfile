FROM php:7.4.0-fpm

RUN apt update && apt install -y \
    libicu-dev \
    libonig-dev \
    zip \
    unzip \
    libpq-dev
RUN pecl install xdebug
RUN docker-php-ext-install intl \
    && docker-php-ext-install pcntl \
    && docker-php-ext-install pdo_mysql \
    && docker-php-ext-enable xdebug

RUN ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime
