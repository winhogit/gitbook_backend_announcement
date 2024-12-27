---
description: 取出單一公告區塊關聯站台資料
---

# fetchSites()

```php
public fetchSites(int $announcementId): DBCollection
```

#### Parameters

| type | name            | comment |
| ---- | --------------- | ------- |
| int  | $announcementId | 公告 id   |

#### **Return Value**

<table><thead><tr><th width="357">type</th><th>comment</th></tr></thead><tbody><tr><td>Illuminate\Database\Eloquent\Collection</td><td>公告區塊關聯站台集合<br>[ { id, name }, { id, name }, .... ]</td></tr></tbody></table>
