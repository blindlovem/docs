---
title: 恋爱盲盒
language_tabs:
  - shell: Shell
  - http: HTTP
  - javascript: JavaScript
  - ruby: Ruby
  - python: Python
  - php: PHP
  - java: Java
  - go: Go
toc_footers: []
includes: []
search: true
code_clipboard: true
highlight_theme: darkula
headingLevel: 2
generator: "@tarslib/widdershins v4.0.22"

---

# 恋爱盲盒

Base URLs:

# Authentication

# 用户信息相关

## POST 添加用户信息

POST /user/user

添加用户信息

> Body Parameters

```json
{}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## PUT 修改信息

PUT /user/{id}

修改信息

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer| yes |用户id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## GET 查询指定用户

GET /user/{id}

查询指定用户

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer| yes |用户id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## GET 查询全部

GET /user

查询全部

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

# 情话

## GET 点击按钮弹出三句情话。

GET /romantic

点击按钮弹出三句情话。

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## GET 返回id用户匹配到过的所有用户

GET /romantic/{id}

返回id用户匹配到过的所有用户

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer| yes |用户id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## POST 点击发送后：保存发送记录

POST /sendword/sendword

点击发送后：保存发送记录

> Body Parameters

```json
{}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 成功

```json
true
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## DELETE 删除一条记录

DELETE /sendword/{id}

删除一条记录

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer| yes |记录id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## GET 用户点击时，就会弹出收到的消息

GET /sendword/{id}

用户点击时，就会弹出收到的消息

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer| yes |用户id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## GET 智能推荐情话

GET /test/{id}

智能推荐情话

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer| yes |用户id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

# 匹配

## POST 寻缘：匹配，选出一个最佳对象(根据算法)

POST /pickrecord/pickrecord

寻缘：匹配，选出一个最佳对象(根据算法)

> Body Parameters

```json
{}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## GET 查询id对应的情话内容

GET /pickrecord/{id}

查询id对应的情话内容

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer| yes |情话id|

> Response Examples

> 成功

```json
"情话对象"
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

# 照片

## POST 上传照片

POST /photos/file

上传照片

> Body Parameters

```yaml
file: string

```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|
|» file|body|string(binary)| no |上传的文件照片|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## GET 查看照片

GET /photos/{id}

查看照片

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer| yes |用户id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## DELETE 删除照片

DELETE /photos/{id}

删除照片

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer| yes |用户id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

# 收藏

## POST 新增：用户点击收藏，存储下来

POST /collection/collection

新增：用户点击收藏，存储下来

> Body Parameters

```json
{}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## GET 查询用户收藏的礼物

GET /collection/{id}

查询用户收藏的礼物

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer| yes |用户id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## DELETE 根据collection表的主键删除收藏记录

DELETE /collection/{id}

根据collection表的主键删除收藏记录

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|string| yes |收藏记录id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

# 盲盒记录

## GET 查询用户id对应的投递记录

GET /blindbox/{id}

查询用户id对应的投递记录

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer| yes |用户id|

> Response Examples

> 成功

```json
"记录列表"
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## POST 添加投递的盲盒记录

POST /blindbox/blindbox

添加投递的盲盒记录

> Body Parameters

```json
{}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## DELETE 删除指定的盲盒（根据盲盒id删除）即：删除一条投递记录

DELETE /bindbox/{id}

删除指定的盲盒（根据盲盒id删除）即：删除一条投递记录

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|string| yes |盲盒id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

# 礼物

## GET 查询所有广告信息

GET /advertisements

查询所有广告信息

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## GET 相应点击广告事件，点击次数加1，并且返回广告详情

GET /advertisements/{id}

相应点击广告事件，点击次数加1，并且返回广告详情

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|integer| yes |礼物id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

## GET 根据关键词查询

GET /advertisements/key

根据关键词查询

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|key|query|string| no |关键词|

> Response Examples

> 成功

```json
"礼物列表"
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

# 八字算命

## GET 八字算命

GET /bazi/{id}

八字算命

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|path|string| yes |用户id|

> Response Examples

> 成功

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### Responses Data Schema

# Data Schema

