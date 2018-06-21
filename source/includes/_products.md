
# Products


## list

```shell
curl "http://api.talkpal.com/products"
  -H "Authorization: Bearer TOKEN"
```

> The above command returns JSON structured like this:

```json
{
	"data": [
		{
			"id": 24,
			"name": "pig",
			"description": null,
			"price": "100.0",
			"currency": "RMB",
			"count_on_hand": null,
			"properties": null,
			"images": [
				{
					"id": 1,
					"alt": "Funny pig",
					"position": 1,
					"small_url": "http://0.0.0.0:3000/rails/active_storage/representations/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBJZz09IiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--1a6055009a4c9e3a3927170f6cc8ccbb24bcb419/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdCam9MY21WemFYcGxTU0lOTVRBd2VERXdNRDRHT2daRlZBPT0iLCJleHAiOm51bGwsInB1ciI6InZhcmlhdGlvbiJ9fQ==--b6d0bf94dbc07dd002d54da460e24210143911a7/170.png",
					"normal_url": "http://0.0.0.0:3000/rails/active_storage/representations/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBJZz09IiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--1a6055009a4c9e3a3927170f6cc8ccbb24bcb419/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdCam9MY21WemFYcGxTU0lOTWpRd2VESTBNRDRHT2daRlZBPT0iLCJleHAiOm51bGwsInB1ciI6InZhcmlhdGlvbiJ9fQ==--b0eea37a6c03f6c4a139066d0e0dcb63cebdb901/170.png",
					"large_url": "http://0.0.0.0:3000/rails/active_storage/representations/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBJZz09IiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--1a6055009a4c9e3a3927170f6cc8ccbb24bcb419/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdCam9MY21WemFYcGxTU0lOTmpBd2VEWXdNRDRHT2daRlZBPT0iLCJleHAiOm51bGwsInB1ciI6InZhcmlhdGlvbiJ9fQ==--2dee6e9af6e3b61f113bd88daa15bc0bce3bd2d8/170.png"
				},
				{
					"id": 2,
					"alt": "Funny pig",
					"position": 2,
					"small_url": "http://0.0.0.0:3000/rails/active_storage/representations/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBJdz09IiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--1ff0301c1d4028544bc587d3bad554710b3dc643/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdCam9MY21WemFYcGxTU0lOTVRBd2VERXdNRDRHT2daRlZBPT0iLCJleHAiOm51bGwsInB1ciI6InZhcmlhdGlvbiJ9fQ==--b6d0bf94dbc07dd002d54da460e24210143911a7/hCB8ZoJNUuy1ghjdDNKzmyog.png",
					"normal_url": "http://0.0.0.0:3000/rails/active_storage/representations/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBJdz09IiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--1ff0301c1d4028544bc587d3bad554710b3dc643/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdCam9MY21WemFYcGxTU0lOTWpRd2VESTBNRDRHT2daRlZBPT0iLCJleHAiOm51bGwsInB1ciI6InZhcmlhdGlvbiJ9fQ==--b0eea37a6c03f6c4a139066d0e0dcb63cebdb901/hCB8ZoJNUuy1ghjdDNKzmyog.png",
					"large_url": "http://0.0.0.0:3000/rails/active_storage/representations/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBJdz09IiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--1ff0301c1d4028544bc587d3bad554710b3dc643/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdCam9MY21WemFYcGxTU0lOTmpBd2VEWXdNRDRHT2daRlZBPT0iLCJleHAiOm51bGwsInB1ciI6InZhcmlhdGlvbiJ9fQ==--2dee6e9af6e3b61f113bd88daa15bc0bce3bd2d8/hCB8ZoJNUuy1ghjdDNKzmyog.png"
				}
			]
		}
	]
}
```

This endpoint list all products.

### HTTP Request

`GET https://api.talkpal.com/products`




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
     -F "product[name]=toy" \
     -F "product[description]=goodboy" \
     -H "Authorization: Bearer TOKEN"
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "id": 1,
		"name": "toy",
		"description": "goodboy",
		"price": "100.0",
		"currency": "RMB",
		"count_on_hand": null,
		"properties": null,
  }
}
```

This endpoint create a product.


### HTTP Request

`POST https://api.talkpal.com/products`

### Product Parameters

Parameter | Required | Description
--------- | --------- | -----------
name | Yes | product name
description | No | product description
price | Yes | prodct price
currency | Yes | currency




## update

```shell
curl -X PATCH https://api.talkpal.com/products/1 \
     -F "product[name]=toy1" \
     -H "Authorization: Bearer TOKEN"
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "id": 1,
		"name": "toy1",
		"description": "goodboy",
		"price": "100.0",
		"currency": "RMB",
		"count_on_hand": null,
		"properties": null,
  }
}
```

This endpoint update a product.

### HTTP Request

`PATCH https://api.talkpal.com/products/<ID>`


### URL Parameters

Parameter | Required | Description
--------- | --------- | -----------
ID | Yes | The ID of the product to retrieve


### Product Parameters

Parameter | Required | Description
--------- | --------- | -----------
name | Yes | product name
description | No | product description
price | Yes | prodct price
currency | Yes | currency





## delete

```shell
curl -X DELETE "http://api.talkpal.com/products/1"
  -H "Authorization: Bearer TOKEN"
```


This endpoint delete a specific product.


### HTTP Request

`DELETE https://api.talkpal.com/products/<ID>`

### URL Parameters

Parameter | Required | Description
--------- | --------- | -----------
ID | Yes | The ID of the product to delete







## add image

```shell
curl -X POST https://api.talkpal.com/products \
     -F "product_image[alt]=Funny" \
     -F "product_image[attachment]=@/Users/cj/Desktop/5vvyo4u8y8wz.jpg" \
     -H "Authorization: Bearer TOKEN"
```

> The above command returns JSON structured like this:

```json
{
	"data": {
		"id": 2,
		"alt": "Funny",
		"position": 2,
		"small_url": "http://0.0.0.0:3000/rails/active_storage/representations/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBJdz09IiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--1ff0301c1d4028544bc587d3bad554710b3dc643/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdCam9MY21WemFYcGxTU0lOTVRBd2VERXdNRDRHT2daRlZBPT0iLCJleHAiOm51bGwsInB1ciI6InZhcmlhdGlvbiJ9fQ==--b6d0bf94dbc07dd002d54da460e24210143911a7/hCB8ZoJNUuy1ghjdDNKzmyog.png",
		"normal_url": "http://0.0.0.0:3000/rails/active_storage/representations/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBJdz09IiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--1ff0301c1d4028544bc587d3bad554710b3dc643/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdCam9MY21WemFYcGxTU0lOTWpRd2VESTBNRDRHT2daRlZBPT0iLCJleHAiOm51bGwsInB1ciI6InZhcmlhdGlvbiJ9fQ==--b0eea37a6c03f6c4a139066d0e0dcb63cebdb901/hCB8ZoJNUuy1ghjdDNKzmyog.png",
		"large_url": "http://0.0.0.0:3000/rails/active_storage/representations/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBJdz09IiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--1ff0301c1d4028544bc587d3bad554710b3dc643/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdCam9MY21WemFYcGxTU0lOTmpBd2VEWXdNRDRHT2daRlZBPT0iLCJleHAiOm51bGwsInB1ciI6InZhcmlhdGlvbiJ9fQ==--2dee6e9af6e3b61f113bd88daa15bc0bce3bd2d8/hCB8ZoJNUuy1ghjdDNKzmyog.png"
	}
}
```

This endpoint create a product image.

### HTTP Request

`POST https://api.talkpal.com/products/<ProductID>/images`

### URL Parameters

Parameter | Required | Description
--------- | --------- | -----------
ProductID | Yes | product ID

### Product image Parameters

Parameter | Required | Description
--------- | --------- | -----------
alt | No | alternative text
attachment | Yes | file to upload







## list images

```shell
curl -X GET https://api.talkpal.com/products/1/image \
     -H "Authorization: Bearer TOKEN"
```

> The above command returns JSON structured like this:

```json
{
	"data": [
		{
			"id": 1,
			"alt": "Funny pig",
			"small_url": "http://0.0.0.0:3000/rails/active_storage/representations/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBJZz09IiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--1a6055009a4c9e3a3927170f6cc8ccbb24bcb419/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdCam9MY21WemFYcGxTU0lOTVRBd2VERXdNRDRHT2daRlZBPT0iLCJleHAiOm51bGwsInB1ciI6InZhcmlhdGlvbiJ9fQ==--b6d0bf94dbc07dd002d54da460e24210143911a7/170.png",
			"normal_url": "http://0.0.0.0:3000/rails/active_storage/representations/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBJZz09IiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--1a6055009a4c9e3a3927170f6cc8ccbb24bcb419/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdCam9MY21WemFYcGxTU0lOTWpRd2VESTBNRDRHT2daRlZBPT0iLCJleHAiOm51bGwsInB1ciI6InZhcmlhdGlvbiJ9fQ==--b0eea37a6c03f6c4a139066d0e0dcb63cebdb901/170.png",
			"large_url": "http://0.0.0.0:3000/rails/active_storage/representations/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaHBJZz09IiwiZXhwIjpudWxsLCJwdXIiOiJibG9iX2lkIn19--1a6055009a4c9e3a3927170f6cc8ccbb24bcb419/eyJfcmFpbHMiOnsibWVzc2FnZSI6IkJBaDdCam9MY21WemFYcGxTU0lOTmpBd2VEWXdNRDRHT2daRlZBPT0iLCJleHAiOm51bGwsInB1ciI6InZhcmlhdGlvbiJ9fQ==--2dee6e9af6e3b61f113bd88daa15bc0bce3bd2d8/170.png"
		}
	]
}
```

This endpoint list all images of a product.

### HTTP Request

`GET https://api.talkpal.com/products/<ProductID>/images`

### URL Parameters

Parameter | Required | Description
--------- | --------- | -----------
ProductID | Yes | product ID
