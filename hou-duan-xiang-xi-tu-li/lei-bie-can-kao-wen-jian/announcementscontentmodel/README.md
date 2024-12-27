---
description: 後台公告區塊內容資料模組
---

# AnnouncementsContentModel

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
protected string $table = 'announcements_content';
protected array $fillable = [
    'announcement_id',
    'backend_lang',
    'title',
    'content',
];
```

### Methods

* [relatedAnnouncement()](relatedannouncement.md)
