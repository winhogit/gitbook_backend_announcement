---
description: 後台公告區塊關聯站台模組
---

# AnnouncementsSites

### Namespace

```php
App\Models
```

### Imports

無

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
protected string $table = 'announcements_sites';
protected array $fillable = [
    'announcement_id',
    'site_id',
];
```

### Methods

* [relatedAnnouncement()](../announcementscontent/relatedannouncement.md)
