# Users

## Show User

```shell
curl "http://api.talkpal.com/users/2" \
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

### HTTP Request

`GET https://api.talkpal.com/users/<ID>`

### URL Parameters

Parameter | Required | Description
--------- | --------- | -----------
ID | Yes | The ID of the user to retrieve


## Update User

```shell
curl  -X PATCH "http://api.talkpal.com/users/1218" \
  -F "user[username]=alice" \
  -H "Authorization: Bearer TOKEN"
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "id": 1218,
    "username": "alice"
  }
}
```

### HTTP Request

`PATCH https://api.talkpal.com/users/<ID>`

### URL Parameters

Parameter | Description
--------- | ---------
ID        | The ID of the user to update

### User Parameters

Parameter | Description
--------- | --------- 
username  | 用户名
profile_image | 头像





