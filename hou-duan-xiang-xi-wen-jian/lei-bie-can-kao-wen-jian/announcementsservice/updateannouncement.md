---
description: 建立、更新，單一公告區塊資料
---

# updateAnnouncement()

```php
public updateAnnouncement(?int $announcementId, bool $status, bool $allSites, bool $allBackendLang): DBCollection
```

#### Parameters

| type      | name            | comment          |
| --------- | --------------- | ---------------- |
| int\|null | $announcementId | 公告 id；新建公告留空     |
| bool      | $status         | 啟用狀態；預設 false    |
| bool      | $allSites       | 全站台顯示狀態；預設 false |
| bool      | $allBackendLang | 全語系顯示狀態；預設 false |

#### **Return Value**

<table><thead><tr><th width="359">type</th><th>comment</th></tr></thead><tbody><tr><td>Illuminate\Database\Eloquent\Collection</td><td><p>公告區塊資料</p><p>{ id, status, all_sites, all_lang }</p></td></tr></tbody></table>
