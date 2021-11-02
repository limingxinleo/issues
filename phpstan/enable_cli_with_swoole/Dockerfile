FROM hyperf/hyperf:8.0-alpine-v3.14-swoole

WORKDIR /opt/www

ADD . .

RUN composer update -o \
    && vendor/bin/phpstan analyse -l 5 -c phpstan.neon index.php
