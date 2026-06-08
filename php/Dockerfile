FROM php:8.3.28-apache 

 

# Instala y habilita la extensión mysqli 

RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli 

 

# Copia la aplicación al contenedor 

COPY index.php /var/www/html/index.php

 

# Establece permisos 

RUN chown -R www-data:www-data /var/www/html/pinacoteca

RUN chmod -R 755 /var/www/html/pinacoteca

 

# Expone el puerto 80 

EXPOSE 80 