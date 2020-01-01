FROM php:7.3-apache

RUN mkdir /app

WORKDIR /app

COPY docker/vhost.conf /etc/apache2/sites-available/000-default.conf

# changing the ownership of the application files to the apache web server
RUN chown -R www-data:www-data /app && a2enmod rewrite

COPY . /app/