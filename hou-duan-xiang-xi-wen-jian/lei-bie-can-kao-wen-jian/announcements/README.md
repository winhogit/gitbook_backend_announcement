---
description: 後台公告資料模組
---

# Announcements

### Namespace

```php
App\Models
```

### Imports

```php
Illuminate\Database\Eloquent\SoftDeletes
```

### Inheritance

```php
Illuminate\Database\Eloquent\Model
```

### Traits

```php
App\Traits\ModelTrait
```

### Dependencies

無

### Properties

```php
protected string $table = 'announcements';
protected array $fillable = [
    'status',
    'all_site',
    'all_lang',
];
protected array $casts = [
    'status' => 'boolean',
    'all_site' => 'boolean',
    'all_lang' => 'boolean',
];
protected array $hidden = [
    'relatedContent',
    'relatedSites',
];
```

### Methods

* [relatedContent()](relatedcontent.md)
* [relatedSites()](relatedsites.md)
* [getContentAttribute()](getcontentattribute.md)
* [getSitesAttribute()](getsitesattribute.md)
