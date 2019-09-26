# 参加该房间内的小电视抽奖

## 参加抽奖

### REQUEST
- Website: https://live.bilibili.com/6
- Method: **POST**
- URL: `https://api.live.bilibili.com/xlive/lottery-interface/v5/smalltv/join`
- Headers:
  - Cookie
  - PC-header
- data
```json5
{
  "id": 1495008,  // raffle_id
  "roomid": 47377,  // real_roomid
  "type": "small_tv",  // raffle_type
  "csrf_token": "*******",  // token
  "csrf": "*******",  // token 同上
  "visit_id": "",  // 应该用于追踪，实际情况感觉无卵用，可以不加这个东西
}
```

### RESPONSE
- 返回数据0
```json5
{
  "code":0,
  "data":{
    "id":432242,
    "award_id":1,
    "award_type":0,
    "award_num":1,  // award_num
    "award_image":"http://i0.hdslb.com/bfs/live/***.png",
    "award_name":"辣条",  // award_name
    "award_text":"",
    "award_ex_time":1572019200,},
  "message":"",
  "msg":"",
}
```
- 返回数据1
```json5
{
  "code":-403,
  "data":null,
  "message":"您已参加抽奖~",
  "msg":"您已参加抽奖~",
}
```
- 返回数据2
```json5
{
  "code": -401,
  "data": null,
  "message": "抽奖还没开始哦, 请耐心等待~",
  "msg": "抽奖还没开始哦, 请耐心等待~",
}
```
- 返回数据3
```json5
{
  "code":-405,
  "data":null,
  "message":"奖品都被领完啦！下次下手快点哦~",
  "msg":"奖品都被领完啦！下次下手快点哦~",
}
```
- 返回数据4
```json5
{
  "code": -403,
  "data": null,
  "message": "访问被拒绝",
  "msg": "访问被拒绝",
}
```