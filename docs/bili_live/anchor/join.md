# 参加该房间内的天选抽奖

## 参加抽奖

### REQUEST
- Website: https://live.bilibili.com/6
- Method: **POST**
- URL: `https://api.live.bilibili.com/xlive/lottery-interface/v1/Anchor/Join`
- Headers:
  - Cookie
  - PC-header
- data
```json5
{
  "id": 34946,  // raffle_id
  "platform": "pc",  // real_roomid,
  "csrf_token": "*******",  // token
  "csrf": "*******",  // token 同上
  "visit_id": "",  // 应该用于追踪，实际情况感觉无卵用，可以不加这个东西
}
```

### RESPONSE
- 返回数据0
```json5
{
	"code": 0,
	"data": null,
	"message": "",
	"msg": ""
}
```

- 返回数据1
```json5
{
	"code": 400,
	"data": null,
	"message": "粉丝勋章等级不满足要求哦",
	"msg": "粉丝勋章等级不满足要求哦"
}
```

