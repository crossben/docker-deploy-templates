# Use official PHP Apache base image
# this is the same as symfony/6 and symfony/7 unless you want to use a different PHP version then change 8.1 to your desired version
FROM php:8.1-apache

# Install dependencies and PHP extensions needed for Symfony
RUN apt-get update && apt-get install -y \
    git \
    unzip \
    zip \
    curl \
    libicu-dev \
    libpq-dev \
    libzip-dev \
    libonig-dev \
    && docker-php-ext-install intl pdo pdo_mysql zip opcache

# Enable Apache mod_rewrite
RUN a2enmod rewrite

# Set working directory inside the container
WORKDIR /var/www/html

# Copy project files (can be skipped if using volume)
COPY . /var/www/html

# Set permissions (adjust as needed for your Symfony setup)
# if this does not work, you might need to connect to the container and run these commands manually
# docker exec -it your-container-name or id bash , then run the commands below
RUN chown -R www-data:www-data /var/www/html \
    && chmod -R 775 /var/www/html/var

# Install Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# Expose Apache port
EXPOSE 80

# Start Apache
CMD ["apache2-foreground"]
