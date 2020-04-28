# Easily raise validation error with custom message

When dealing with complex validation scenarios it is often beneficial to raise the validation exception manually. Or there may be some scenarios where you can't do a validation before doing a lot of other actions or queries.

It is as simple as throwing a `Illuminate\Validation\ValidationException`:

```php
use Illuminate\Validation\ValidationException;

throw ValidationException::withMessages(['field_name' => 'This value is incorrect']);
```

[Source](https://stackoverflow.com/questions/47219542/how-can-i-manually-return-or-throw-a-validation-error-exception-in-laravel)
