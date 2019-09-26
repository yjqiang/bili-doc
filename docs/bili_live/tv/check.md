# 获取该房间内的小电视抽奖

## 获取抽奖

### REQUEST
- Website: https://live.bilibili.com/6
- Method: **GET**
- URL: `https://api.live.bilibili.com/xlive/lottery-interface/v1/lottery/Check?roomid={real_roomid}`
- Headers:
  - No Cookie
  - Header can be empty
  
### RESPONSE
- 返回数据0
```json5
{
  "code": 0,
  "message": "0",
  "ttl": 1,
  "data": {
    "pk": [],
    "guard": [],
    "gift": [
      {
        "raffleId": 427839,  // raffle_id
        "type": "small_tv",  // join 需要这个东西作为参数
        "from_user": {
          "uid": 0,
          "uname": "大鹅在敬老院给你留锅",
          "face": "http://i1.hdslb.com/bfs/face/***.jpg"},
        "time_wait": 6,  // 当前到可以参与最少等待时间
        "time": 66,  // 当前到可以参与最大等待时间
        "max_time": 180,
        "status": 1,
        "sender_type": 0,
        "asset_icon": "http://s1.hdslb.com/bfs/live/***.png",
        "asset_animation_pic": "http://i0.hdslb.com/bfs/live/***.gif",
        "thank_text": "感谢\u003c%大鹅在敬老院给你留锅%\u003e 赠送的小电视飞船",
        "weight": 0,
        "gift_id": 25}],
  },
}
```
  
 