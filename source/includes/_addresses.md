# Addresses

## 获取用户的收货地址

```shell
curl "http://api.talkpal.com/addresses"
  -H "Authorization: Bearer TOKEN"
```

> The above command returns JSON structured like this:

```json
{
	"data": [
		{
			"id": 1,
			"province": "guang dong",
			"city": "guang zhou",
			"district": null,
			"street": null,
			"line1": null,
			"postal_code": null,
			"phone_number": null,
			"full_name": "guolijun",
			"position": 1
		}
	]
}
```

### HTTP Request

`GET https://api.talkpal.com/addresses`




## 添加地址

```shell
curl -X POST "http://api.talkpal.com/addresses"
  -H "Authorization: Bearer TOKEN"
```

> The above command returns JSON structured like this:

```json
{
	"data": {
		"id": 2,
		"province": "广东",
		"city": "广州",
		"district": null,
		"street": null,
		"line1": null,
		"postal_code": null,
		"phone_number": null,
		"full_name": "guolijun",
		"position": 2
	}
}
```


### HTTP Request

`POST https://api.talkpal.com/address`

### Address Parameters

Parameter | Description
--------- | -----------
province  |    省
city	|	      市
district |	    区或县
street	|	    街道或乡镇
line1	|	      地址
postal_code	|  邮政编码
phone_number | 联系人手机号
full_name |  联系人姓名
