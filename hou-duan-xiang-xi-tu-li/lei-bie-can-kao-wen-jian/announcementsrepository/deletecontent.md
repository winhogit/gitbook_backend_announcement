---
description: 刪除公告區塊內容
---

# deleteContent()

{% code fullWidth="false" %}
```php
public deleteContent(int $announcementId, string $backendLang): DBCollection
```
{% endcode %}

#### Parameters

| type   | name            | comment  |
| ------ | --------------- | -------- |
| int    | $announcementId | 公告 id    |
| string | $backend\_lang  | 公告區塊內容語系 |

#### **Return Value**

<table data-full-width="false"><thead><tr><th width="371">type</th><th>comment</th></tr></thead><tbody><tr><td>Illuminate\Database\Eloquent\Collection</td><td>公告區塊內容集合<br>[ { id, announcement_id, backend_lang, title, content }, ....  ]</td></tr></tbody></table>
