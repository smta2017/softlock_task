FROM php:7.4-fpm

 
WORKDIR /var/www/html
# COPY ./../../ /var/www/html

# Install dependencies for the operating system software
RUN apt-get update && apt-get install -y \
    # build-essential \
    # libpng-dev \
    # libjpeg62-turbo-dev \
    # libfreetype6-dev \
    # libcurl4-openssl-dev \
    # pkg-config \
    # libssl-dev \
    # locales \
    zip \
    # jpegoptim optipng pngquant gifsicle \
    # vim \
    # libzip-dev \
    unzip \
    git 
    # libonig-dev \
    # curl
    # nodejs \
    # npm

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# RUN docker-php-ext-install mysqli pdo pdo_mysql

RUN chown -R www-data:www-data /var/www/html

# RUN compose update

EXPOSE 9000