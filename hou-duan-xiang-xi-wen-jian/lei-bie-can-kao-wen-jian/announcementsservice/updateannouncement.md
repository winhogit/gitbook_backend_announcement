---
description: 建立、更新，單一公告區塊資料
---

# updateAnnouncement()



```php
public updateAnnouncement(?int $announcementId, bool $status, bool $allSites, bool $allLang, array $contents, array $sites): DBCollection
```

#### Parameters

| type      | name            | comment          |
| --------- | --------------- | ---------------- |
| int\|null | $announcementId | 公告 id；新建公告留空     |
| bool      | $status         | 啟用狀態；預設 false    |
| bool      | $allSites       | 全站台顯示狀態；預設 false |
| bool      | $allLang        | 全語系顯示狀態；預設 false |
| array     | $contents       | 公告區塊內容陣列         |
| int\[]    | $sites          | 站台 id 陣列         |

#### **Return Value**

<table><thead><tr><th width="359">type</th><th>comment</th></tr></thead><tbody><tr><td>Illuminate\Database\Eloquent\Collection</td><td><p>公告區塊資料</p><p>{ id, status, all_sites, all_lang }</p></td></tr></tbody></table>
