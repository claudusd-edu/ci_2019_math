FROM php:8.0.2-cli

RUN apt update && apt install -y git zlib1g-dev libzip-dev

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

RUN  docker-php-ext-install bcmath zip