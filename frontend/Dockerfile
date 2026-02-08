# frontend/Dockerfile
FROM php:8.2-apache

# Copiamos todo el contenido del frontend
COPY . /var/www/html/

# Damos permisos correctos
RUN chown -R www-data:www-data /var/www/html \
    && chmod -R 755 /var/www/html

# Activamos rewrite si el frontend es SPA, opcional pero util
RUN a2enmod rewrite

EXPOSE 80