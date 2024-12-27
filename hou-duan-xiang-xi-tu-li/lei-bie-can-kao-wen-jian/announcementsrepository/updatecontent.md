---
description: 更新公告區塊內容
---

# updateContent()

{% code fullWidth="false" %}
```php
public updateContent(string $title, string $content, string $backendLang, ?int $announcementId): DBCollection
```
{% endcode %}

#### Parameters

| type      | name            | comment      |
| --------- | --------------- | ------------ |
| string    | $title          | 公告區塊抬頭       |
| string    | $content        | 公告區塊內文       |
| string    | $backendLang    | 公告區塊內容語系     |
| int\|null | $announcementId | 公告 id；新建內容留空 |

#### **Return Value**

<table data-full-width="false"><thead><tr><th width="371">type</th><th>comment</th></tr></thead><tbody><tr><td>Illuminate\Database\Eloquent\Collection</td><td>公告區塊內容集合<br>[ { id, announcement_id, backend_lang, title, content }, ....  ]</td></tr></tbody></table>
