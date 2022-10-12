FROM php:8.1.10-apache

# Enable ssl module for apache
RUN a2enmod ssl

# COPY ./httpd-conf/httpd.conf /usr/local/apache2/conf/httpd.conf
# COPY ./httpd-conf/ssl.conf /usr/local/apache2/conf/extra/httpd-ssl.conf

# Add vertualhost configuration
COPY ./httpd-conf/virtualhost.conf /etc/apache2/sites-available/000-default.conf

# Add ssl key and sertificate
# COPY ./certs/name.crt /etc/ssl/name.crt
# COPY ./certs/name.key /etc/ssl/name.key

# informe Docker that the container listen port 443 (https)
EXPOSE 443