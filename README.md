# netmusic-node
网易音乐接口node版
``` bash
# 下载项目到本地
git clone git@github.com:sqaiyan/netmusic-node.git

cd netmusic-node 

# 安装依赖
npm install 

# 启动项目 服务器中可用pm2或foreve之类
node app.js | pm2 app.js

```

## 前端请求
```
Axios("http://localhost:3000/v1/music/detail?id=276830");
```
### 响应
```
[
    {
        "name": "盛夏的果实(Live) - live",
        "id": 276830,
        "pst": 0,
        "t": 0,
        "ar": [
            {
                "id": 8926,
                "name": "莫文蔚",
                "tns": [],
                "alias": []
            }
        ],
        "alia": [],
        "pop": 100,
        "st": 0,
        "rt": "600902000000028747",
        "fee": 8,
        "v": 22,
        "crbt": null,
        "cf": "",
        "al": {
            "id": 27493,
            "name": "回蔚 巡回演唱会(台北)",
            "picUrl": "http://p1.music.126.net/vhP4I5u6LMQxPHPHUY8_aQ==/68169720934925.jpg",
            "tns": [],
            "pic": 68169720934925
        },
        "dt": 286537,
        "h": {
            "br": 320000,
            "fid": 0,
            "size": 11475716,
            "vd": 0
        },
        "m": {
            "br": 160000,
            "fid": 0,
            "size": 5750199,
            "vd": 0
        },
        "l": {
            "br": 96000,
            "fid": 0,
            "size": 3459574,
            "vd": -0.000265076
        },
        "a": null,
        "cd": "1",
        "no": 5,
        "rtUrl": null,
        "ftype": 0,
        "rtUrls": [],
        "djId": 0,
        "copyright": 1,
        "s_id": 0,
        "rurl": null,
        "rtype": 0,
        "cp": 7003,
        "mst": 9,
        "mv": 0,
        "publishTime": 1333036800000
    }
]
```
更多接口见app.js。其他接口可看web官网js源码。客户端可抓包分析


## 注意
接口调用是有频率限制的,搜索，歌单类请求太频繁会返回空数据，登录类直接封IP，部署在vps要小心开放访问

## 应用实例
[网易云音乐-微信小程序](https://github.com/sqaiyan/NeteaseMusicWxMiniApp)

[网易云音乐-Vue高仿ios客户端](https://github.com/sqaiyan/neteasemusic)
