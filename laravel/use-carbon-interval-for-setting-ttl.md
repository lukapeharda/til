# Use `CarbonInterval` instead of magic numbers for setting up TTL

Don't use magic numbers when defining any TTL (like cache or cookies) in PHP (especially in Laravel projects). Use human-readable intervals instead using `CarbonInterval`.

```php
// Instead of
Cache::put('key', 'value', 60 * 60 * 24 * 7);
// or
cookie('key', 'value', 60 * 24 * 30);

// Rater use more readable
Cache::put('key', 'value', CarbonInterval::week()->totalSeconds);
// and
cookie('key', 'value', CarbonInterval::days(30)->totalMinutes);
```

[Source](https://carbon.nesbot.com/docs/#api-interval)
