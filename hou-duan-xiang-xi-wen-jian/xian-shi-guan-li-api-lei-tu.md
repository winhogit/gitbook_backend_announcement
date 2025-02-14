# 顯示、管理 API 類圖

<figure><img src="../.gitbook/assets/WinShop 後台公告類圖.png" alt=""><figcaption></figcaption></figure>

```mermaid
---
title: WinShop 後台公告類圖
config:
  theme: dark
  darkMode: true
---
classDiagram
    AnnouncementsController ..> AnnouncementsService
    AnnouncementsService ..> AnnouncementsRepository
    AnnouncementsRepository ..> Announcements
    AnnouncementsRepository ..> AnnouncementsContent
    AnnouncementsRepository ..> AnnouncementsSites
    Announcements "1" o-- "1..*" AnnouncementsContent
    Announcements "1" o-- "0..*" AnnouncementsSites
    namespace App.Http.Controllers.Api.Backend {
        class AnnouncementsController {
            <<Controller>>
            # AnnouncementsService $announcementsService
            + __construct()
            + display()
            + list()
            + fetch()
            + createAnnouncement()
            + updateAnnouncement()
            + deleteAnnouncement()
        }
    }
    namespace App.Services {
        class AnnouncementsService {
            <<Service>>
            # AnnouncementsRepository $announcementsRepository
            + __construct()
            + display()
            + list(int $page, int $rows)
            + fetch(int $announcementId)
            + updateAnnouncement(?int $announcementId, bool $status, bool $allSites, bool $allLang, array $contents, array $sites)
            + deleteAnnouncement(int $announcementId)
        }
    }
    namespace App.Repositories {
        class AnnouncementsRepository {
            <<Repository>>
            + __construct()
            + factory()
            + status()
            + updateContent(string $title, string $content, string $backendLang, int $announcementId)
            + deleteContent(int $announcementId, string $backendLang)
            + updateSites(int $announcementId, array $siteIds)
            + deleteAnnouncement(int $announcementId)
        }
    }
    namespace App.Models {
        class Announcements {
            <<Model>>
            # string $table
            # array $fillable
            # array $casts
            # array $appends
            # array $hidden
            + relatedContent()
            + relatedSites()
            + getTitleAttribute()
            + getContentAttribute()
            + getContentsAttribute()
            + getSitesAttribute()
            - getDisplayContent()
        }
        class AnnouncementsContent {
            <<Model>>
            # string $table
            # array $fillable
            # array $hidden
            + relatedAnnouncement()
        }
        class AnnouncementsSites {
            <<Model>>
            # string $table
            # array $fillable
            # array $hidden
            + relatedAnnouncement()
            + relatedSite()
        }
    }
```
