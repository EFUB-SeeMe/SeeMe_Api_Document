---
description: 시간대별 강수량을 알려주는 api
---

# 시간대별 강수량

## 1) URL

```
GET /weather/rain
```

## 2) RESPONSE BODY

### Success http status code

HTTP Status code: `200 OK`

### Description

|  name   |  type  | description |
| :-----: | :----: | :---------- |
|  time   | string | 시간        |
|  rain   |  int   | 강수량      |
| percent |  int   | 강수 확률   |
|  icon   | string | 아이콘 URL  |

### Example

```json
{
	[
        {
            "time": 12,
            "rain": 30,
            "percent": 60,
            "icon": "https://user-images.githubus{ercontent.com/68107000/174224687-19f86b00-db41-11eb-9090-d2b32f38fa67.png"
        },
        {
            "time": 12,
            "rain": 30,
            "percent": 60,
            "icon": "https://user-images.githubusercontent.com/68107000/174224687-19f86b00-db41-11eb-9090-d2b32f38fa67.png"
        },
        {
            "time": 12,
            "rain": 30,
            "percent": 60,
            "icon": "https://user-images.githubusercontent.com/68107000/174224687-19f86b00-db41-11eb-9090-d2b32f38fa67.png"
        },
        {
            "time": 12,
            "rain": 30,
            "percent": 60,
            "icon": "https://user-images.githubusercontent.com/68107000/174224687-19f86b00-db41-11eb-9090-d2b32f38fa67.png"
        },
        {
            "time": 12,
            "rain": 30,
            "percent": 60,
            "icon": "https://user-images.githubusercontent.com/68107000/174224687-19f86b00-db41-11eb-9090-d2b32f38fa67.png"
        }
	]
}
```

## 3) ERROR CODE

| error code | error message           | description    |
| :--------- | :---------------------- | :------------- |
| 500        | INTERNAL\_SERVER\_ERROR | 서버 내부 에러 |
