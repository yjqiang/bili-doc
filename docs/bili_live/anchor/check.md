# 获取该房间内的天选抽奖

## 获取抽奖

### REQUEST
- Website: https://live.bilibili.com/6
- Method: **GET**
- URL: `https://api.live.bilibili.com/xlive/lottery-interface/v1/Anchor/Check?roomid={real_roomid}`
- Headers:
  - No Cookie
  - Header can be empty
  
### RESPONSE
- 返回数据0.0
```json5
{
	"code": 0,
	"data": {
		"id": 34946,
		"room_id": 8182490,
		"status": 1,
		"asset_icon": "https://i0.hdslb.com/bfs/live/992c2ccf88d3ea99620fb3a75e672e0abe850e9c.png",
		"award_name": "5元红包",
		"award_num": 1,
		"award_image": "",
		"danmu": "66666",
		"time": 203,
		"current_time": 1577621606,
		"join_type": 0,
		"require_type": 1,
		"require_value": 0,
		"require_text": "关注主播",
		"gift_id": 0,
		"gift_name": "",
		"gift_num": 1,
		"gift_price": 0,
		"cur_gift_num": 0,
		"goaway_time": 180,
		"award_users": [],
		"show_panel": 1,
		"url": "https://live.bilibili.com/p/html/live-lottery/anchor-join.html?is_live_half_webview=1&hybrid_biz=live-lottery-anchor&hybrid_half_ui=1,5,100p,100p,000000,0,30,0,0,1;2,5,100p,100p,000000,0,30,0,0,1;3,5,100p,100p,000000,0,30,0,0,1;4,5,100p,100p,000000,0,30,0,0,1;5,5,100p,100p,000000,0,30,0,0,1;6,5,100p,100p,000000,0,30,0,0,1;7,5,100p,100p,000000,0,30,0,0,1;8,5,100p,100p,000000,0,30,0,0,1",
		"lot_status": 0,
		"web_url": "https://live.bilibili.com/p/html/live-lottery/anchor-join.html",
		"send_gift_ensure": 0
	},
	"message": "ok",
	"msg": "ok"
}
```

- 返回数据0.1
```json5
{
    "code": 0,
    "data": {
        "id": 25396,
        "room_id": 10556121,
        "status": 1,
        "asset_icon": "https://i0.hdslb.com/bfs/live/992c2ccf88d3ea99620fb3a75e672e0abe850e9c.png",
        "award_name": "照片",
        "award_num": 1,
        "award_image": "",
        "danmu": "咩",
        "time": 270,
        "current_time": 1576809967,
        "join_type": 1,
        "require_type": 0,
        "require_value": 0,
        "require_text": "无",
        "gift_id": 30046,
        "gift_name": "打榜",
        "gift_num": 1,
        "gift_price": 2000,
        "cur_gift_num": 0,
        "goaway_time": 180,
        "award_users": [
            
        ],
        "show_panel": 1,
        "url": "https://live.bilibili.com/p/html/live-lottery/anchor-join.html?is_live_half_webview=1&hybrid_biz=live-lottery-anchor&hybrid_half_ui=1,5,100p,100p,000000,0,30,0,0,1;2,5,100p,100p,000000,0,30,0,0,1;3,5,100p,100p,000000,0,30,0,0,1;4,5,100p,100p,000000,0,30,0,0,1;5,5,100p,100p,000000,0,30,0,0,1;6,5,100p,100p,000000,0,30,0,0,1;7,5,100p,100p,000000,0,30,0,0,1;8,5,100p,100p,000000,0,30,0,0,1",
        "lot_status": 0,
        "web_url": "https://live.bilibili.com/p/html/live-lottery/anchor-join.html",
        "send_gift_ensure": 0
    },
    "message": "ok",
    "msg": "ok"
}
```

- 返回数据0.2
```json5
{
	"code": 0,
	"data": {
		"id": 34528,
		"room_id": 15536,
		"status": 1,
		"asset_icon": "https://i0.hdslb.com/bfs/live/992c2ccf88d3ea99620fb3a75e672e0abe850e9c.png",
		"award_name": "明日方舟限定家具兑换码",
		"award_num": 1,
		"award_image": "",
		"danmu": "抽奖",
		"time": 160,
		"current_time": 1577622607,
		"join_type": 0,
		"require_type": 2,
		"require_value": 1,
		"require_text": "当前主播粉丝勋章至少1级",
		"gift_id": 0,
		"gift_name": "",
		"gift_num": 1,
		"gift_price": 0,
		"cur_gift_num": 0,
		"goaway_time": 180,
		"award_users": [],
		"show_panel": 1,
		"url": "https://live.bilibili.com/p/html/live-lottery/anchor-join.html?is_live_half_webview=1&hybrid_biz=live-lottery-anchor&hybrid_half_ui=1,5,100p,100p,000000,0,30,0,0,1;2,5,100p,100p,000000,0,30,0,0,1;3,5,100p,100p,000000,0,30,0,0,1;4,5,100p,100p,000000,0,30,0,0,1;5,5,100p,100p,000000,0,30,0,0,1;6,5,100p,100p,000000,0,30,0,0,1;7,5,100p,100p,000000,0,30,0,0,1;8,5,100p,100p,000000,0,30,0,0,1",
		"lot_status": 0,
		"web_url": "https://live.bilibili.com/p/html/live-lottery/anchor-join.html",
		"send_gift_ensure": 0
	},
	"message": "ok",
	"msg": "ok"
}
```

- 返回数据1
```json5
{
	"code": 0,
	"data": null,
	"message": "ok",
	"msg": "ok"
}
```
 