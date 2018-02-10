
# laravel-cheatsheet
laravel 5.5 cheatsheet


## **Eloquent: API Resources**

    php artisan make:resource UserCollection
    php artisan make:resource Users --collection
    use App\Http\Resources\UserResource;

## **Defining Models**

    php artisan make:model User

**Create a model with migration**

    php artisan make:model User --migration
    php artisan make:model User -m
