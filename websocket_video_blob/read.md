html5 video blob demo
* nodejs 读取 mp4fragment websockt 推流
* 前端将二进制视频流喂给 video blob

nodejs 8.10 +
浏览器桌面版

-----------------------------------------------------------------------
nodejs 环境安装
1.apt-get install nodejs 或者 brew install nodejs 或者 win10 msi
2.建立软连接 sudo ln -s /usr/bin/nodejs /usr/bin/node 
3.node -v查看版本号

npm nodejs 包管理器安装 并换国内淘宝源 cnpm
1.apt-get install npm 或者 brew install npm
2.npm install -g cnpm --registry=https://registry.npm.taobao.org
或者
npm set registry https://registry.npm.taobao.org # 注册模块镜像
npm set disturl https://npm.taobao.org/dist # node-gyp 编译依赖的 node 源码镜像
npm cache clean --force # 清空缓存

利用 n模块 升级 nodejs 版本 目前的 lts8.10
1.cnpm install n
2.n stable

-----------------------------------------------------------------------
运行 demo
1.clone到本地 并 cd 文档
2.执行 npm install 安装依赖（ws／uuid／buffer模块）
2.node main.js 默认端口号80
websocket端口1999 默认本地网络pi.local或者自行修改页面index的ws链接地址