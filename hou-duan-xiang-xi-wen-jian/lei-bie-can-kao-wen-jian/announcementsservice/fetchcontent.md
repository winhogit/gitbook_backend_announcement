---
description: 取出單一公告區塊各語系內容資料
---

# fetchContent()

```php
public fetchContent(int $announcementId): DBCollection
```

#### Parameters

| type | name            | comment |
| ---- | --------------- | ------- |
| int  | $announcementId | 公告 id   |

#### **Return Value**

<table><thead><tr><th width="359">type</th><th>comment</th></tr></thead><tbody><tr><td>Illuminate\Database\Eloquent\Collection</td><td>公告區塊內容集合<br>[ { id, announcement_id, backend_lang, title, content }, ....  ]</td></tr></tbody></table>
