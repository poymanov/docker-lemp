FROM php:7.2-fpm

RUN apt-get update && apt-get install -y \
        curl \
    && docker-php-ext-install mysqli pdo_mysql

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

WORKDIR /var/www

CMD ["php-fpm"]
