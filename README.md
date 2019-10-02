# Laravel Menu Builder
Laravel Menu Builder with VueJs and jQuery.

#Install the Package

```
composer require codexshaper/laravel-menu-builder
```
#Publish Resource, Configs, Migration and Seeding Database in a single command

```
php artisan menu:install
```
#run `php artisan serve`

#for check menus go to `http://127.0.0.1:8000/admin/menus` . You can change `admin` prefix from `config/menu.php`

#How to use Menu in your site?
1. Call Menu anywhere on your site by calling `{{ menu('name') }}` or `@menu('name')`
2. Link CSS and JS if you want to use our default design 
```
CSS: <link rel="stylesheet" type="text/css" href="{{ menu_asset('css/menu.css') }}">
JS: <script src="{{ menu_asset('js/menu.js') }}"></script> 
```
3. Optional: If you don't have jQuery and bootstrap in your page then add bellow files before above CSS and Js
```
CSS: <link rel="stylesheet" type="text/css" href="{{ menu_asset('css/app.css') }}">
JS: <script src="{{ menu_asset('js/menu.js') }}"></script>
```