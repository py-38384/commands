**Linking Storage public folder to Publick folder**

```
php artisan storage:link
```

**Migrating and refreshing and seeding**
```
php artisan migrate:refresh --seed
```

**Making a factory to seed data with a model**
```
php artisan make:factory <FactoryName> --model=<model_name>
```
**Creating a controller and CRUD functionality barebone with a model** 
```
php artisan make:controller <ControllerName> --resource --model=<model_name>
```

**Creting View**
```
php artisan make:view <folder_name>.<view_name>
```
----
### To connect postgres DB from artisan

* goto "php.init"
* uncomment thoes

    **extension=pdo_pgsql**
    *extension=pgsql**


All CRUD related route compact in one Route

```php
Route::resource('<model_name>', <ControllerName>::class);
```