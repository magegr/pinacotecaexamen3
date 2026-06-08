FROM php:8.3-apache

# Instala la extensión mysqli
RUN docker-php-ext-install mysqli

# Crea la carpeta del endpoint
RUN mkdir -p /var/www/html/pinacoteca

# Copia la aplicación dentro de /pinacoteca
COPY index.php /var/www/html/pinacoteca/index.php

# Establece permisos
RUN chown -R www-data:www-data /var/www/html
RUN chmod -R 755 /var/www/html

# Expone el puerto 80
EXPOSE 80