FROM php:7.1-fpm

RUN pecl install xdebug
RUN docker-php-ext-enable xdebug

COPY ./php.ini /etc/php/7.1/fpm/conf.d/40-custom.ini

# Install composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer