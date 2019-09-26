# 参加该房间内的大乱斗抽奖

## 参加抽奖

### REQUEST
- Website: https://live.bilibili.com/6
- Method: **POST**
- URL: `https://api.live.bilibili.com/xlive/lottery-interface/v2/pk/join`
- Headers:
  - Cookie
  - PC-header
- data
```json5
{
  "id": 480023,  // raffle_id
  "roomid": 1259929,  // real_roomid
  "type": "pk",  // raffle_type
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
  "message":"0",
  "ttl":1,
  "data":{
    "id":480023,
    "award_id":1,
    "award_type":0,
    "award_num":1,  // award_num
    "award_image":"https://i0.hdslb.com/bfs/live/***.png",
    "award_name":"",
    "award_text":"辣条X1",
    "award_ex_time":1570032000,
  },
}
```
- 返回数据1
```json5
{
  "code":-2,
  "data":null,
  "message":"您已参加过抽奖",
  "msg":"您已参加过抽奖",
}
```
- 返回数据2
```json5
{
  "code":-1,
  "data":null,
  "message":"抽奖已结束",
  "msg":"抽奖已结束",
}
```
- 返回数据3
```
TODO
```
