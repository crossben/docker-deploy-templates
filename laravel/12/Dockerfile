# Use the official PHP image with Apache
FROM php:8.2-apache

WORKDIR /var/www

# Install system dependencies
# this use PostgreSQL, if you want to use mySQL, replace libpq-dev and pdo_pgsql with libmysql-dev and pdo_mysql
RUN apt-get update && apt-get install -y \
    libpng-dev \
    libjpeg62-turbo-dev \
    libfreetype6-dev \
    libzip-dev \
    unzip \
    git \
    zip \
    curl \
    libpq-dev \
    postgresql-client \
    && rm -rf /var/lib/apt/lists/*

# Install PHP extensions including PostgreSQL
RUN docker-php-ext-configure gd --with-freetype --with-jpeg \
    && docker-php-ext-install gd pdo pdo_pgsql zip

# Enable Apache mod_rewrite for Laravel routing
RUN a2enmod rewrite

# Set Apache DocumentRoot to Laravel public folder
RUN sed -i 's|DocumentRoot /var/www/html|DocumentRoot /var/www/public|g' /etc/apache2/sites-available/000-default.conf

# Copy app files
COPY . /var/www

# Install Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# Install Laravel dependencies
RUN composer install --no-interaction --prefer-dist

# Laravel caching and optimization
RUN php artisan config:cache \
    && php artisan route:cache \
    && php artisan view:cache 

# Fix permissions
# if this does not work, you might need to connect to the container and run these commands manually
# docker exec -it your-container-name or id bash , then run the commands below
RUN chown -R www-data:www-data /var/www/storage /var/www/bootstrap/cache \
    && chmod -R 775 /var/www/storage /var/www/bootstrap/cache

# Ensure this is the same port as defined in your docker-compose file
EXPOSE 80 
