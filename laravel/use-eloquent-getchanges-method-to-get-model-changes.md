# Use Eloquent's `getChanges` method to get model changes

After saving (or updating) your Eloquent model you can easily get list of change attributes and its new data even after they were synced to the DB.

```php

$dummyModel = DummyModel::create([
  'foo' => 'bar',
  'bar' => 'baz',
]);

$dummyModel->update([
  'foo' => 'baz',
]);

$changes = $dummyModel->getChanges();

// $changes are equal to Array(['foo' => 'baz']);  
```

There are several other interesting methods regarding changes in the `Illuminate\Database\Eloquent\Concerns\HasAttributes` trait:

* `wasChanged($attributes = null)` where you can check if there are any changes or whether any specific (or many specific) attributes have changed
* `hasChanges($changes, $attributes = null)` which checks if any of the given attributes were changed

While checking this methods out be sure to check family of `dirty` methods to check for changes before DB sync.
