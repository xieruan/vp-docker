## V2Ray Plugin For V2Board
###安装docker
  
```bash

curl -fsSL https://get.docker.com | bash
curl -L "https://github.com/docker/compose/releases/download/1.25.3/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod a+x /usr/local/bin/docker-compose
# 创建个软链接，以后用 dc 命令来代替 docker-compose
rm -rf `which dc`  # 若系统中存在 dc 则删除，这个 dc 就是个计算器，完全没有用
ln -s /usr/local/bin/docker-compose /usr/bin/dc

```
###下载

```bash

git clone https://github.com/xieruan/vp-docker.git
```
配置docker-compose.yml和config.json

###启动docker
```bash
dc up
```
