>>>> Formação PHP Experience <<<<

## Laravel: Construindo uma API do Zero
Por: Roberto Oliveira

- composer install
- php artisan key:generate  
- php artisan migrate
- php artisan serve

## Prerequisitos
- PHP 7.1 or Higher
- Composer
- MySql
- Laravel 5.6 or Higher (laravel/framework": "5.7.*)
- Postman

## API CRUD
GET /api/students
GET /api/students/{id}
POST /api/students
PUT /api/students/{id}
DELETE /api/students/{id}

```
Route::get('students', 'ApiController@getAllStudents');
Route::get('students/{id}', 'ApiController@getStudent');
Route::post('students, 'ApiController@createStudent');
Route::put('students/{id}', 'ApiController@updateStudent');
Route::delete('students/{id}','ApiController@deleteStudent');
```

## Modelo de resultado

```
[
    {
        "id": 1,
        "name": "Roberto Oliveira",
        "course": "DIO",
        "created_at": "2023-06-05 15:10:12",
        "updated_at": "2023-06-05 14:10:12"
    }
]
```

