# Specify Columns While Eager Loading

While eager loading eloquent relationships using `with` method you can specify ("select") which columns you want to have returned:

```php
User::where(...)->with('business:id,name')->get()
```

Mind you, `id` is required in order for relationship matching to work.

This is available in Laravel since version 5.3.

[Source](https://github.com/laravel/framework/pull/16327)
