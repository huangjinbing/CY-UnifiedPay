# Logout - 登出

**应用场景**

该接口提供用户登出。

**校验签名**

> 否

**接口链接**

> [http://{BaseURL}/](http://{BaseURL}/OpenPlatform/Login)[Manage](http://{BaseURL}/OpenPlatform/Login)[/Logout](http://{BaseURL}/OpenPlatform/Login)

**提交方式**

> POST

**请求参数**

| 参数 | 必填 | 示例值 | 说明 |
| :--- | :--- | :--- | :--- |
| user\_id | 是 | 00000000000000000000000000000000 | 用户Id |
| token | 是 | 00000000000000000000000000000000 | Token令牌 |

**请求参数示例**

> user\_id=00000000000000000000000000000000&token=00000000000000000000000000000000

**响应结果**

| 字段名 | 必填 | 说明 |
| :--- | :--- | :--- |
| code | 是 | 状态码 ，详见参数规定 |
| msg | 否 | 返回信息 |
| data | 否 | 响应数据 |

以下字段在code为SUCCESS的时候在data参数中返回

| 字段名 | 必填 | 说明 |
| :--- | :--- | :--- |
| redirect\_uri | 否 | 回调地址 |

**响应结果示例**

```js
{
    "code": "SUCCESS",
    "msg": "SUCCESS",
    "data": "{\"redirect_uri\":\"http://{BaseURL}/Manage/Login\"}"
}
```



