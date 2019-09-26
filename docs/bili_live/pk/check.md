# 获取该房间内的大乱斗抽奖

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
  "code":0,
  "message":"0",
  "ttl":1,
  "data":{
    "pk":[
      {
        "id":480011,
        "pk_id":480011,
        "room_id":4960254,
        "time":48,  // 当前到可以参与最大等待时间
        "status":1,
        "asset_icon":"https://i0.hdslb.com/bfs/vc/***.png",
        "asset_animation_pic":"https://i0.hdslb.com/bfs/vc/***.gif",
        "max_time":120,
        "time_wait":0,  // 当前到可以参与最少等待时间
        "from_user":{
          "uid":29312803,
          "uname":"幽螟蛉",
          "face":"http://i0.hdslb.com/bfs/face/***.jpg"},
        "thank_text":"恭喜\u003c%幽螟蛉%\u003e赢得大乱斗PK胜利",
        "weight":0}],
    "guard":[],
    "gift":[],
  },
}
```
  
 