# Advanced Streaming Tech

## Week 2

- Php lecture for OOP

## Week 3

- Nothing

## Week 4

- Open Lab

## Week 5

- Laravel Beginning
  - Installed Laravel via composer
  - `composer global require laravel/installer`
  - Created via `composer create-project --prefer-dist laravel/laravel blog`
  - Served via `php artisan serve`
  - Created controller via `php artisan make:controller AsdfController -r`

## Week 8

- Migrations in Laravel
  - Move and maintain structure in Laravel without dumping & reimporting
- Migrations are created in a similar way to M2 upgrade files
- By default, a table will us the snake case plural name of a class for a model
  - IE a model MyItem extends Model will have a table my_item

## Week 9

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
