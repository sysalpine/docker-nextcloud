FROM nextcloud:15.0.7-fpm

ENV PHP_MEMORY_LIMIT=512M
COPY nextcloud.ini /usr/local/etc/php/conf.d/nextcloud.ini

COPY user.ini /var/www/html/.user.ini
