# Learning Laravel

Useful Links and Artisan Commands for Laravel.

## Useful links

Laravel:
https://laravel.com/

Composer:
https://getcomposer.org/

Laravel Cheat Sheet:
http://cheats.jesse-obrien.ca/

## Database, Mail, Environment Settings

File: .env

## Forms and Html

https://laravelcollective.com/docs/5.4/html#installation
```
1. step: composer.json: "require": "laravelcollective/html":"^5.4.0" 
2. step: composer update 
3. step: config/app.php:	'providers' => 'Collective\Html\HtmlServiceProvider'
		'aliases' => 'Form' => 'Collective\Html\FormFacade'
		'Html' => 'Collective\Html\HtmlFacade'
```

## Installing Laravel
```
composer create-project --prefer-dist laravel/laravel (folder name) / Folder will be created in the directory you specify
```

## Artisan Commands

**Listing all commands:**
```
php artisan list
```

**Creating all of the routes and views you need for authentication:**
```
php artisan make:auth
```

**Creating a controller:**
```
php artisan make:controller (controller name)
```

**Creating a controller which contains a method for each of the available resource operations:**
```
php artisan make:controller (controller name) --resource
```

**Creating a model instance:**
```
php artisan make:model (model name)
```

**Creating Form Requests:**
```
php artisan make:request (request name)
```

**Creating Database Migrations:**
```
php artisan make:migration create_(table name)_table
```

**Run all outstanding migrations:**
```
php artisan migrate
```

**Rollback the latest migration operation:**
```
php artisan migrate:rollback
```
