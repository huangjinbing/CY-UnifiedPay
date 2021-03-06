# Login - 登录

**应用场景**

该接口提供用户验证，获取Token，并完成通过Token进行后续的业务逻辑。

**校验签名**

> 否

**接口链接**

> [http://{BaseURL}/Manage/Login](http://{BaseURL}/OpenPlatform/Login)

**提交方式**

> POST

**请求参数**

| 参数 | 必填 | 示例值 | 说明 |
| :--- | :--- | :--- | :--- |
| account | 是 | aaa | 帐号 |
| pwd | 是 | bbb | 密码 |

**请求参数示例**

> account=aaa&pwd=bbb

**响应结果**

| 字段名 | 必填 | 说明 |
| :--- | :--- | :--- |
| code | 是 | 状态码 ，详见参数规定 |
| msg | 否 | 返回信息 |
| data | 否 | 响应数据 |

以下字段在code为SUCCESS的时候在data参数中返回

| 字段名 | 必填 | 说明 |
| :--- | :--- | :--- |
| user\_id | 是 | 用户Id |
| real\_name | 是 | 昵称 |
| head\_img | 否 | 头像图片地址 |
| token | 是 | Token令牌 |

**响应结果示例**

```js
{
    "code": "SUCCESS",
    "msg": "SUCCESS",
    "data": "{\"user_id\":\"00000000000000000000000000000000\",\"real_name\":\"aaa\",\"token\":\"00000000000000000000000000000000\"}"
}
```



