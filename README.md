# Laravel-QuickStart
Quickstart Task List in Laravel

https://laravel.com/docs/5.1/quickstart

- Made migration for table `php artisan make:migration create_tasks_table --create=tasks`
- added new column string('name') to tasks table
- updated .env file with mysql test user and db
- ran php artisan migrate to database tables
- php artisan make:model Task (Eloquent Models)
- Model placed in app directory  
- Assumes Task is `tasks`  
- https://laravel.com/docs/5.1/eloquent

# Routes
- routes/web.php
- added Route::post and Route::delete
- added return view(...);
- use App\\Task;
-- For Model Class Namespace  
- use Illuminate\\Http\\Request;
-- For Http Post Request

# Views
- This application only has a single view which contains a form for adding new tasks as well as a listing of all current tasks. To help you visualize the view, here is a screenshot of the finished application with basic Bootstrap CSS styling applied:

![Finished App](http://laravel.com/assets/img/quickstart/basic-overview.png)

- Shared Blade Layouts
- resources/views/layouts/app.blade.php
- @yield('content')
- child view
- views/tasks.blade.php
- @extends('layouts.app') @section('content')
