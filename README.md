# laravel-cheatsheet

laravel 5.5 cheatsheet

## **Eloquent: API Resources**

```
php artisan make:resource UserCollection
php artisan make:resource Users --collection
use App\Http\Resources\UserResource;
```

## **Defining Models**

```
php artisan make:model User
```

**Create a model with migration**

```
php artisan make:model User --migration
php artisan make:model Score -m
```

**Filter collection with starts_with**

```
$form_data=collect(json_decode($request->form_data, true));
$exeption_color_types =  $form_data->filter(function ($item) {
            return starts_with($item['name'], 'exeption_');
});
```

## **Create a new controller with resource**

```
php artisan make:controller UserController --resource
```
