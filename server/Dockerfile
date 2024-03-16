FROM php:8.3.3-apache

RUN apt-get update \
# && apt-get install -y apt-utils curl sqlite3 \
&& pecl install xdebug

ADD ./php.ini /usr/local/etc/php/

ADD ./sites /etc/apache2/sites-available

RUN a2ensite httpd.conf

EXPOSE 80
