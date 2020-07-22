FROM php:7.4-fpm-alpine3.12

WORKDIR /var/www/mystery_logger

RUN apk add --update --no-cache postgresql-dev
RUN docker-php-ext-install pgsql pdo_pgsql
RUN mkdir -p /var/lib/php/session

CMD [ "php-fpm" ]
