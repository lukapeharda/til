# Use `Builder::toBase` method to return `stdClass` object from your query

Use `Illuminate\Database\Eloquent\Builder::toBase` method when you want or need to return `stdClass` from you query instead of the model class:

```php
$user = App\User::find(1); // $user is an instance of App\User

$user = App\User::toBase()→find(1); // $user is an instance of stdClass
```

This can be useful in queries where you are modifying the select part of the query and returning aggregates or some computed values.
