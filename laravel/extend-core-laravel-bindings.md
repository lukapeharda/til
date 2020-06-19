# Extend core Laravel bindings

Within the container, Laravel defines an extend method that lets you extend services in the container. The extend method takes the service you want to extend as the first argument and a Closure as the second. The Closure should run additional code to modify or decorate the service. It receives the original service and an instance of the container and should return the modified service.

```php
app()->extend('service', function ($service, $app) {
    return new DecoratedService($service);
});
```

`DecoratedService` now extends `Service` and provides added functionality to it.

[Source](https://medium.com/@orobogenius/extending-core-laravel-bindings-97f409140fc3)
