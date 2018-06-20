
# Products

## show

```shell
curl "http://api.talkpal.com/products/1"
  -H "Authorization: Bearer TOKEN"
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "id": 1,
		"name": "toy 101",
		"description": null,
		"price": "100.0",
		"currency": "RMB",
		"count_on_hand": null,
		"properties": null,
  }
}
```

This endpoint retrieves a specific product.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET https://api.talkpal.com/products/<ID>`

### URL Parameters

Parameter | Required | Description
--------- | --------- | -----------
ID | Yes | The ID of the product to retrieve


## create

```shell
curl -X POST https://api.talkpal.com/products \
     -F "image[name]=toy" \
     -F "image[images][]=@/Users/cj/Desktop/5vvyo4u8y8wz.jpg" \
     -H "Authorization: Bearer TOKEN"
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "id": 1,
		"name": "toy 101",
		"description": null,
		"price": "100.0",
		"currency": "RMB",
		"count_on_hand": null,
		"properties": null,
  }
}
```

This endpoint create a product.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`POST https://api.talkpal.com/products`

### Product Parameters

Parameter | Required | Description
--------- | --------- | -----------
name | Yes | product name
price | Yes | prodct price
currency | Yes | currency

