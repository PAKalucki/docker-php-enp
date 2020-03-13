FROM nginx:latest

ARG PHP_HOST
ENV PHP_HOST $PHP_HOST

COPY index.php /var/www/html/index.php
COPY default.conf /etc/nginx/conf.d/default.conf
RUN sed -i "s/@PHP_HOST@/$PHP_HOST/g" /etc/nginx/conf.d/default.conf