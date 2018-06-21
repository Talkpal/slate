# Orders

## Create Order

下单

### HTTP Request

`POST https://api.talkpal.com/orders`

### URL Parameters

Parameter       | Description
---------       | -----------
product         | 产品类型: goods 或 subscription
product_id      | 产品 ID
address_id      | 收货地址, 产品类型是 goods 时，该参数必须。





## List Orders

获取用户的历史订单

### HTTP Request

`GET https://api.talkpal.com/orders`

### URL Parameters

Parameter | Description
--------- | -----------
category  | 产品分类：goods 或者 subscription


