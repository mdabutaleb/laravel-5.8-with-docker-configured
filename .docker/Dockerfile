FROM php:7.2-apache

COPY . /srv/app
COPY .docker/vhost.conf /etc/apache2/sites-available/000-default.conf

RUN apt-get update && \
        apt-get install -y \
            zlib1g-dev

RUN docker-php-ext-install mbstring pdo pdo_mysql mysqli zip


RUN chown -R www-data:www-data /srv/app \
        && a2enmod rewrite


