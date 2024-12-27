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
Kalnoy\Nestedset\Collection
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
* [list()](list.md)
* [fetch()](fetch.md)
* [fetchContent()](fetchcontent.md)
* [fetchSites()](fetchsites.md)
* [updateAnnouncement()](updateannouncement.md)
