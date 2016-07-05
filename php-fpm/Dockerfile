FROM php:fpm-alpine

RUN apk add --no-cache \
        autoconf \
        build-base && \

    docker-php-ext-install pdo pdo_mysql && \
    pecl install xdebug  && \
    docker-php-ext-enable xdebug && \

     apk del \
            autoconf \
            build-base