# laravel-commands

- php artisan make:model --migration --controller Template --resource

- php artisan migrate
- php artisan migrate:fresh
- php artisan migrate:reset
- php artisan migrate:rollback --step=1
- php artisan migrate --path=/database/migrations/2021_02_03_064125_create_media_table.php

- php artisan config:cache
- php artisan config:clear
- php artisan cache:clear

- composer dump-auto
- php artisan cache:clear && php artisan config:clear && php artisan config:cache && php artisan key:generate
    
    


- sudo find . -type d -exec chmod 0755 {} \;
- sudo find . -type f -exec chmod 0644 {} \;
- COMPOSER_MEMORY_LIMIT=-1 composer require spatie/laravel-s
- php artisan make:migration create_contact_table
- php artisan migrate:rollback --step=1
- php artisan db:seed --class=PermissionSeeder
- php artisan make:model Contact
- php artisan make:middleware Frontend
- php artisan make:controller Admin/SubCategories


#LINUX SERVER USER PERMISION TO A FOLDER
- sudo chown -R ubuntu:www-data .env
- sudo chown -R daemon:daemon storage/*

#There is no permission named `admin.users.getUsers` for guard `web`
- php artisan cache:forget spatie.permission.cache && php artisan cache:clear


#remove last merge code command
- git reset --hard HEAD^

#Gmail 2-step verification

- 1. enable the 2-step verification to google HERE

- 2. Create App Password to be use by your system HERE

- 3. select Others (custom name) and clicked generate

- 4. go to env file in laravel and edited this

- MAIL_USERNAME=yourid@gmail.com

- MAIL_PASSWORD=thepasswordgenerated

# Database group by error
- SET GLOBAL sql_mode=(SELECT REPLACE(@@sql_mode,'ONLY_FULL_GROUP_BY',''));

# Linux Commands
- sudo apt-get install php-curl
- sudo apt install zip unzip php-zip
- sudo chown -R www-data:www-data storage/
- sudo chown -R www-data:www-data storage/*

# PHP VERSION
- AddHandler application/x-httpd-php74 .php

# Argument list too long error for rm, cp, mv commands
- find . -maxdepth 1 -name '*.json' -delete

# Simply use the following command,

- For Export:

- mysqldump -u [user] -p [db_name] | gzip > [filename_to_compress.sql.gz] 
- For Import:

- gunzip < [compressed_filename.sql.gz]  | mysql -u [user] -p[password] [databasename] 


#Freelancer Ubantu 64bit .deb

  https://s3.amazonaws.com/desktop-production.freelancer.com/latest/installers/freelancer-desktop-app_ubuntu-amd64.deb

# <a target="_blank" href="https://www.digitalocean.com/community/tutorials/how-to-rewrite-urls-with-mod_rewrite-for-apache-on-ubuntu-18-04"> refrence </a>  if dynamic url not found on server, run sudo nano /etc/apache2/sites-available/000-default.conf, then sudo systemctl restart apache2
    <VirtualHost *:80> 
       <Directory /var/www/html>
          Options Indexes FollowSymLinks MultiViews
          AllowOverride All
          Require all granted
       </Directory>
      . . .
    </VirtualHost>   


