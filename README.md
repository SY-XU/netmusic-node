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



详细接口见app.js。更多接口可看web官网js源码。客户端可抓包分析


## 注意
接口调用是有频率限制的,搜索，歌单类请求太频繁会返回空数据，登录类直接封IP，部署在vps要小心开放访问

## 应用实例
[网易云音乐-微信小程序](https://github.com/sqaiyan/NeteaseMusicWxMiniApp)

[网易云音乐-Vue高仿ios客户端](https://github.com/sqaiyan/neteasemusic)
