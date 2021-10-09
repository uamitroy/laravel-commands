# laravel-commands

php artisan make:model --migration --controller Template --resource

php artisan migrate
php artisan migrate:fresh
php artisan migrate:reset
php artisan migrate --path=/database/migrations/2021_02_03_064125_create_media_table.php

php artisan config:cache
php artisan config:clear
php artisan cache:clear


sudo find . -type d -exec chmod 0755 {} \;
sudo find . -type f -exec chmod 0644 {} \;
COMPOSER_MEMORY_LIMIT=-1 composer require spatie/laravel-s
php artisan make:migration create_contact_table
php artisan migrate:rollback --step=1
php artisan db:seed --class=PermissionSeeder
php artisan make:model Contact
php artisan make:middleware Frontend
php artisan make:controller Admin/SubCategories


#LINUX SERVER USER PERMISION TO A FOLDER
sudo chown -R ubuntu:www-data .env
sudo chown -R daemon:daemon storage/*


#remove last merge code command
git reset --hard HEAD^
