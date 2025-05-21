# Install php
# If you want to use a different version of PHP, change the PHP_VERSION argument
ARG PHP_VERSION=8.2.28 

FROM php:${PHP_VERSION}-fpm-alpine

# Install system dependencies
RUN apk update && apk add --no-cache \
    libzip-dev \
    libpng-dev \
    libjpeg-turbo-dev \
    libwebp-dev \
    zlib-dev \
    libxml2-dev \
    oniguruma-dev \
    curl \
    git \
    unzip

# Install composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# Install necessary PHP extensions
RUN docker-php-ext-install mysqli \
    pdo \
    pdo_mysql \
    gd \
    zip \
    exif \
    bcmath \
    mbstring