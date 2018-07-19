---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - shell
  - ruby
  - python
  - javascript

toc_footers:
  - <a href='https://www.talkpal.com'>Home</a>
  #- <a href='#'>Sign Up for a Developer Key</a>
  #- <a href='https://github.com/lord/slate'>Documentation Powered by Slate</a>

includes:
  - errors
  - users
  - products
  - addresses
  - orders
  - word_guessing

search: true
---

# Introduction

该文档使用 [Slate](https://github.com/Talkpal/slate) 生成. 你可以 clone 并编辑你需要的 API 文档.

# Scheme
所有 Response 最顶层永远是 JSON 对象 { ... }.
所有成功请求的资源都在 data 字段里.
> 例如请求某用户的用户信息

```json
{
  "data": {
    "id": 98,
    "username": "Zoe"
  }
}
```

> 或者请求课程列表

```json
{
  "data" [
    {"id": 3942, "title": "跟Jeff老师学绘画"},
    {"id": 3942, "title": "跟Mike老师学音乐"}
  ]
}
```

请求出错时参考 [Errors](#errors)

# Authentication

> To authorize, use this code:

```shell
# With shell, you can just pass the correct header with each request
curl "https://api.talkpal.com/sessions"
  -H "Authorization: Bearer TOKEN"
```

> Make sure to replace `TOKEN` with your access token.

Talkpal uses access token to allow access to the API. 

Talkpal expects for the access token to be included in all API requests to the server in a header that looks like the following:

`Authorization: Bearer rNSpfeA_rEv8Tx6n1dnbZ_Uzv8ZA2LLoaeBduj3JGiTeU3ADCkY5AUhQmI1d2tDS3xMoCKv1Rxg9eVtL28tL7Q`

<aside class="notice">
You must replace <code>rNSpfeA_rEv8Tx6n1dnbZ_Uzv8ZA2LLoaeBduj3JGiTeU3ADCkY5AUhQmI1d2tDS3xMoCKv1Rxg9eVtL28tL7Q</code> with your access token.
</aside>

