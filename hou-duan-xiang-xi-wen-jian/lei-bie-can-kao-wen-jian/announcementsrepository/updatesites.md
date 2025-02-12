---
description: 更新公告區塊關聯站台
---

# updateSites()

{% code fullWidth="false" %}
```php
public updateSites(int $announcementId, array $siteIds): DBCollection
```
{% endcode %}

#### Parameters

| type   | name            | comment        |
| ------ | --------------- | -------------- |
| int    | $announcementId | 公告 id          |
| int\[] | $siteIds        | 公告區塊關聯站台 id 陣列 |

#### **Return Value**

<table><thead><tr><th width="357">type</th><th>comment</th></tr></thead><tbody><tr><td>bool</td><td>是否完成</td></tr></tbody></table>
