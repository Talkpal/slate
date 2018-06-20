# Users

## Get a Specific User

```shell
curl "http://api.talkpal.com/users/2"
  -H "Authorization: Bearer TOKEN"
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "id": 1218,
    "username": "Talkpal"
  }
}
```

This endpoint retrieves a specific user.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET https://api.talkpal.com/users/<ID>`

### URL Parameters

Parameter | Required | Description
--------- | --------- | -----------
ID | Yes | The ID of the user to retrieve


## 更新用户信息

```shell
curl  -X PATCH "http://api.talkpal.com/users/2"
  -H "Authorization: Bearer TOKEN"
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "id": 1218,
    "username": "Talkpal"
  }
}
```

### HTTP Request

`PATCH https://api.talkpal.com/users/<ID>`

### URL Parameters

Parameter | Required | Description
--------- | --------- | -----------
ID | Yes | The ID of the user to update



