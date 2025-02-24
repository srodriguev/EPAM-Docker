# Use official WordPress image as base
FROM wordpress:latest

# Set working directory
WORKDIR /var/www/html

# Copy wp-config.php into the container
COPY wp-config.php /var/www/html/

# Ensure correct ownership for WordPress to function properly
RUN chown www-data:www-data /var/www/html/wp-config.php

# Expose port
EXPOSE 80

# Start Apache server
CMD ["apache2-foreground"]