web: vendor/bin/heroku-php-nginx -C nginx_app.conf public/
release: php artisan migrate --force && php artisan cache:clear && php artisan config:cache
worker: php artisan queue:work