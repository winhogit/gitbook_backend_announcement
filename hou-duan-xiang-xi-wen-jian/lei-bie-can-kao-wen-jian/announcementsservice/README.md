---
description: 後台公告資料相關邏輯服務
---

# AnnouncementsService

### Namespace

```php
App\Services
```

### Imports

```php
Illuminate\Pagination\LengthAwarePaginator
Illuminate\Database\Eloquent\Collection as DBCollection
App\Repositories\AnnouncementsRepository
```

### Inheritance

```php
App\Services\AbstractService
```

### Traits

```php
App\Traits\ServiceTrait
```

### Dependencies

```php
App\Repositories\AnnouncementsRepository $announcementsRepository
```

### Properties

無

### Methods

* [\_\_construct()](__construct.md)
* [display()](display.md)
* [list()](list.md)
* [fetch()](fetch.md)
* [updateAnnouncement()](updateannouncement.md)
* [deleteAnnouncement()](deleteannouncement.md)
