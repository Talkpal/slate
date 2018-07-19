# 你说我猜

通过连接 WordGuessing::RoomChannel 和服务器实时通信。

channel 有两个内置的方法 subscribe 和 unsubscribe,可以订阅和取消订阅一个房间的消息.

在该channel上执行action向服务器发送消息。


## query

query(parameters)

parameters: { "query": "<target>", "query_id": 1 }

target 为要查询的目标, 目前仅支持 viewers

query_id 为客户端生成的id,服务器原样返回,客户端可以用来查找回调handler.

> query({"query": "viewers", "query_id": 34})

```json
{ 
    "type": "result",
    "query": "viewers",
    "query_id": 34,
    "viewers": [{"position": 10, "user": {"id": 64, "username", "zoe"}}]
}
```
