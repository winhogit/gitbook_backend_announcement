# 後端 API

## 取得公告區塊列表資料

<mark style="color:green;">`GET`</mark> `/api/shopadmin/announcements`

**Headers**

| Name          | Value              |
| ------------- | ------------------ |
| Content-Type  | `application/json` |
| Authorization | `Bearer <token>`   |

**Body**

| Name   | Type    | Description |
| ------ | ------- | ----------- |
| `page` | integer | 分頁頁次        |
| `rows` | integer | 每頁顯示數量      |

**Response**

{% tabs %}
{% tab title="200" %}
```json
{
  "success": {
    "current_page": 1,
    "data": [
      {
        "id": 1,
        "title": "Announcement title",
        "content": "Announcement content",
        "status": true,
        "all_site": true,
        "all_lang": true
      },
      {
        "id": 2,
        "title": "Announcement title 2",
        "content": "Announcement content 2",
        "status": true,
        "all_site": false,
        "all_lang": true
      },
      ....
    ],
    "per_page": 15,
    "total": 30
  }
}
```
{% endtab %}

{% tab title="401" %}
```json
{
  "error": {
    "message": "Unauthorized"
  }
}
```
{% endtab %}
{% endtabs %}

## 取得公告區塊資料

<mark style="color:green;">`GET`</mark> `/api/shopadmin/announcement`

**Headers**

| Name          | Value              |
| ------------- | ------------------ |
| Content-Type  | `application/json` |
| Authorization | `Bearer <token>`   |

**Body**

| Name | Type    | Description |
| ---- | ------- | ----------- |
| `id` | integer | 公告區塊資料 id   |

**Response**

{% tabs %}
{% tab title="200" %}
```json

{
  "success": {
    {
      "id": 1,
      "title": "Announcement title",
      "content": "Announcement content",
      "status": true,
      "all_site": true,
      "all_lang": true
    }
  }
}
```
{% endtab %}

{% tab title="400" %}
```json
{
  "error": {
    "message": "Unauthorized"
  }
}
```
{% endtab %}
{% endtabs %}

## 建立公告

<mark style="color:green;">`POST`</mark> `/api/shopadmin/announcement`

建立公告資料

**Headers**

| Name          | Value              |
| ------------- | ------------------ |
| Content-Type  | `application/json` |
| Authorization | `Bearer <token>`   |

**Body**

| Name      | Type | Description |
| --------- | ---- | ----------- |
| `sites`   | json | 站台 id json  |
| `status`  | bool | 啟用狀態        |
| all\_site | bool | 全站顯示狀態      |
| all\_lang | bool | 全語系顯示狀態     |

**Response**

{% tabs %}
{% tab title="200" %}
```json
{
  "success": {
    "data": {
      "id": 1,
      "status": true,
      "all_site": false,
      "all_lang": false,
      "created_at": "2024-12-23 00:00:00",
      "updated_at": "2024-12-23 00:00:00",
    },
    "message": "Create complete."
  }
}
```
{% endtab %}

{% tab title="401" %}
```json
{
  "error": {
    "message": "Unauthorized"
  }
}
```
{% endtab %}
{% endtabs %}

