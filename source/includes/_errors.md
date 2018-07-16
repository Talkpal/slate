# Errors

Response 最顶层的 JSON 对象里有些字段是错误信息.

Field   | Description
------- | ---------------
message | 用于显示给用户.
code    | 错误代码,不可变.
errors  | [字段错误](#字段错误)


## 常见错误
客户端使用过程中出现的几类错误.

> 下面的请求将会出错,不存在ID是0的用户.

```shell
curl "http://api.talkpal.com/users/0"
```

```json
{"message": "Not found", "code": "not_found"}
```

Code | Message | Status | Description
---- | ------- | ---------------- | ----------
not_found           | Not found                   | 404 | 未找到请求的资源,通常是因为提供了错误的ID.
not_authenticated   | Not authenticated           | 401 | 用户身份验证失败,通常是提供了错误的 token 
not_authorized      | Not authorized              | 403 | 没有权限访问该资源
token_expired       | The access token expired    | 401 | token 已过期
verification_failed | Incorrect verification code | 403 | 错误的短信验证码

## 字段错误
在创建或更新资源时提供了无效的字段

HTTP Status: 422 Unprocessable Entity

> 创建用户是未填写用户名

```shell
curl -X POST "http://api.talkpal.com/users"
```

```json
{
  "message": "Validation Failed",
  "errors": [
    {
      "resource": "User",
      "field": "username",
      "code": "cant_be_blank"
    }
  ]
}
```

Code          | Description
------------- | -------------
blank         | 字段不能为空
taken         | 该字段的值已经被占用
invalid       | 无效的数据类型

以上字段错误还不完全,待补充.

## 其他错误
当前还有一些在特定的情况下产生的错误,等同于[常见错误](#常见错误)但是还没确定 code, 或者会在后续解决掉的错误.


> 例如: 每日登录奖励已经领取过了

```json
{"message": "The bonus has been taken away"}
```
