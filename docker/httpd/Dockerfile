FROM php:7.4-apache

RUN apt-get update

#Apache2
#file custom host đã thay thế cho file 000-default mặc định của hệ thống được tạo bởi apache2
#nên khi truy cập vào ip của container nó vẫn chạy site này, vì nó đã thay thế file mặc định
RUN a2enmod rewrite && a2enmod ssl
COPY ./000-default.conf /etc/apache2/sites-available