# 查询用户主站相关信息

## 查询当前用户基本信息

### REQUEST
- Website: https://account.bilibili.com/account/home
- Method: **GET**
- URL: `https://account.bilibili.com/home/userInfo`
- Headers:
  - Cookie
  - PC-header
  
### RESPONSE
- 返回数据0
```json5
{
  "code": 0,
  "status": true,
  "data": {
    "level_info": {
      "current_level": 6,  // 当前的等级
      "current_min": 28800,
      "current_exp": 30523,  // 当前实际经验
      "next_exp": -1},  // 该段位的总经验，如果满了就是 -1
    "bCoins": 5,  // B 币
    "coins": 87,
    "face": "http://i2.hdslb.com/bfs/face/***.jpg",  // 头像
    "nameplate_current": "http://i0.hdslb.com/bfs/face/***.png",  // 成就勋章
    "pendant_current": "",
    "uname": "***",  // 用户名
    "userStatus": "正式会员",
    "vipType": 2,
    "vipStatus": 1,
    "official_verify": -1,
    "pointBalance": 100,
  },
}
```
- 返回数据1
```json5
// 登出返回
{"code": -101}
```