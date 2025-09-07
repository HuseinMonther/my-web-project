FROM php:8.2-apache

# انسخ الملفات إلى مجلد الويب داخل Apache
COPY . /var/www/html/

# اجعل Apache يستمع على المنفذ 10000 (مطلوب من Render)
RUN sed -i 's/80/10000/' /etc/apache2/sites-available/000-default.conf

# شغّل Apache في foreground
