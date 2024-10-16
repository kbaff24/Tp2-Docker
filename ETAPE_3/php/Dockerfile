FROM php:8.1-fpm

RUN docker-php-ext-install mysqli pdo pdo_mysql

WORKDIR /var/www/html

RUN curl -O https://wordpress.org/latest.tar.gz && \
    tar -xvzf latest.tar.gz --strip-components=1 && \
    rm latest.tar.gz

RUN chown -R www-data:www-data /var/www/html
