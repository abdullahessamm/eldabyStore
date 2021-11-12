FROM php:8.0-fpm

RUN php -r "copy('https://getcomposer.org/installer', 'composer-installer.php');" && \
    php composer-installer.php --install-dir /usr/local/bin/ --filename composer && \
    php -r "unlink('composer-installer.php');"

WORKDIR /var/www/html