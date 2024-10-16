FROM php:8.1-fpm

RUN docker-php-ext-install mysqli
WORKDIR /app
COPY test_bdd.php .
RUN chown -R www-data:www-data /app
