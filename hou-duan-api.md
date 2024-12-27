# 後端 API

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

