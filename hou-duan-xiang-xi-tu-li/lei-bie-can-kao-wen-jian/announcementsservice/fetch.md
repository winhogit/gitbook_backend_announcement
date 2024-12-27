---
description: 取出單一公告區塊資料
---

# fetch()

```php
public fetch(int $announcementId): DBCollection
```

#### Parameters

| type | name            | comment |
| ---- | --------------- | ------- |
| int  | $announcementId | 公告 id   |

#### **Return Value**

<table><thead><tr><th width="359">type</th><th>comment</th></tr></thead><tbody><tr><td>Illuminate\Database\Eloquent\Collection</td><td><p>公告區塊資料</p><p>{ id, status, all_sites, all_lang }</p></td></tr></tbody></table>
