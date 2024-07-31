# Advanced typed array types

With modern PHP tooling, not only we can do `@param array<Type> $value` but a lot more.

We can specify literal keys:
```php
/**
 * @param array{begin: int, interval: int} $data
 *
 * @return int
 */
function transform(array $data): int {
  return $data['begin'] + $data['interval'];
}
```

The notation for arrays is `array<KeyType, ValueType>`. If we only pass one type, it is the type of the value.

We can even go as far as to specify the array should not be empty:

```php
/**
 * @param non-emptyarray<string, mixed> $data
 *
 * @return non-empty-string
 */
function concatKeys(array $data): string {
  $output = '';
  foreach($data as $key => $v) {
  $output .= $key;
  }
  return $output;
}
```

[Source](https://backendtea.com/post/php-typed-arrays/)