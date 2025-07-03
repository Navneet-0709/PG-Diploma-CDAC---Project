# Dockerfile
FROM php:8.1-apache

# Enable PDO extension for MySQL
RUN docker-php-ext-install pdo pdo_mysql

# Copy app code to web root
COPY . /var/www/html/

# Set proper permissions
RUN chown -R www-data:www-data /var/www/html

# Expose port
EXPOSE 80
