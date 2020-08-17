FROM php:7.2-fpm-alpine

RUN docker-php-ext-install \
    bcmath \
    pdo_mysql \
    opcache

COPY opcache.ini /usr/local/etc/php/conf.d/opcache.ini

RUN curl -fsSL https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
