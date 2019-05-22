# Laravel 5 Repositories

[![Analytics](https://ga-beacon.appspot.com/UA-140657639-1/l5-repository/migration-to-3.0)](https://packagist.org/packages/scolib/l5-repository)

Some changes between version 2.1 and 3.0

## Migrate from version 2.1 to 3.0

### Support Laravel Version

**Not Support Laravel less than 5.5**

```json
  "require": {
    "illuminate/http": "~5.5",
    "illuminate/config": "~5.5",
    "illuminate/support": "~5.5",
    "illuminate/database": "~5.5",
    "illuminate/pagination": "~5.5",
    "illuminate/console": "~5.5",
    "illuminate/filesystem": "~5.5",
    "prettus/laravel-validation": "1.1.*"
  }
```

### Repository method changed

#### v2.1.*

```php
public function firstOrNew(array $attributes = []);
public function firstOrCreate(array $attributes = []);
```



#### v3.0.*

```php
public function firstOrNew(array $attributes, array $values = []);
public function firstOrCreate(array $attributes = [], array $values = []);
```

