# 获取该房间内的大航海抽奖

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
    "guard": [
      {
        "id": 1495083,  // raffle_id
        "sender": {
          "uid": 15258616,
          "uname": "卿茶酒以歌",
          "face": "http://i1.hdslb.com/bfs/face/***.jpg"},
        "keyword": "guard",
        "privilege_type": 2,
        "time": 7075,  // 当前到可以参与最大等待时间
        "status": 1,
        "time_wait": 0,  // 当前到可以参与最少等待时间
        "asset_icon": "https://i0.hdslb.com/bfs/vc/***.png",
        "asset_animation_pic": "https://i0.hdslb.com/bfs/vc/***.gif",
        "thank_text": "恭喜\u003c%卿茶酒以歌%\u003e上任提督",
        "weight": 0}],
    "gift": [],
  },
}
```
  
 