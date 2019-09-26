# 参加该房间内的大航海抽奖

## 参加抽奖

### REQUEST
- Website: https://live.bilibili.com/6
- Method: **POST**
- URL: `https://api.live.bilibili.com/xlive/lottery-interface/v3/guard/join`
- Headers:
  - Cookie
  - PC-header
- data
```json5
{
  "id": 1495008,  // raffle_id
  "roomid": 47377,  // real_roomid
  "type": "guard",  // raffle_type 推测可能就是 check 里面的 keyword 条目
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
  "data": {
    "id": 1495008,  // raffle_id
    "award_id": 0,
    "award_type": 0,
    "award_num": 1,  // award_num
    "award_image": "http://i0.hdslb.com/bfs/live/***.png",
    "award_name": "粉丝勋章亲密度",  // award_name
    "award_text": "粉丝勋章亲密度+1（当前佩戴）",
    "award_ex_time": 0},
  "message": "ok",
  "msg": "ok",
}
```
- 返回数据1
```json5
{
  "code": 400,
  "data": null,
  "message": "你已经领取过啦",
  "msg": "你已经领取过啦",
}
```
- 返回数据2
```json5
{
  "code": 400,
  "data": null,
  "message": "已经过期啦,下次早点吧",
  "msg": "已经过期啦,下次早点吧",
}
```
- 返回数据3
```json5
{
  "code": -403,
  "data": null,
  "message": "访问被拒绝",
  "msg": "访问被拒绝",
}
```
