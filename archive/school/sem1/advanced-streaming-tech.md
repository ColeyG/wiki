# Advanced Streaming Tech

## 2

- Php lecture for OOP

## 3

- Nothing

## 4

- Open Lab

## 5

- Laravel Beginning
  - Installed Laravel via composer
  - `composer global require laravel/installer`
  - Created via `composer create-project --prefer-dist laravel/laravel blog`
  - Served via `php artisan serve`
  - Created controller via `php artisan make:controller AsdfController -r`

## 8

- Migrations in Laravel
  - Move and maintain structure in Laravel without dumping & reimporting
- Migrations are created in a similar way to M2 upgrade files
- By default, a table will us the snake case plural name of a class for a model
  - IE a model MyItem extends Model will have a table my_item

## 9

- Laravel Restful
  - Examples:
    - `Route::get('articles/{artive}', 'ArtivleController@index');`
    - `Route::post('articles/{article}', 'ArticleController@store');`
  - Named Routes:
    - `Route::get('user/profile', 'UserProfileController@show')->name('profile');`
    - `Route::get('user/{id}/profile', function($id) {/** **/})->name('profile');`
  - Creating routes and views without a controller:
    - `Route::get('path', function() {});`
  - Creating route with a controller:
    - `Route::get('agents', AgentController@index);`
  - Controller naming:
    - CamelCase
    - End with Controller
    - SmackTheDomeController
- Seeding
  - Seeding fills a DB with data without manually inputting it
  - database/seeds store seed classes
  - DatabaseSeeder class runs all other seeders
  - Seeder classes only have the run() method
  - `php artisan db:seed`

## 10

- MVC Project
  - Model
  - View
  - Controller
  - Migration
  - Seeder
  - Search Form

- IE:
  - Use a migration to create table of employees
  - Use a seeder to fill employee table
  - Have an employee model
  - Use route facade to create all routes
  - Use the controllers to store your logic to display all necessary views
  - Use blade templates for view files

## 11

- Laravel Auth
  - Made up of Guards and Providers
  - Laravel comes with model and migration for Users
  - requires `composer require laravel/ui`
  - and `php artisan ui vue --auth`
  - and `php artisan migrate`
