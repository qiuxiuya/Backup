## 咸蛋中转面板v1.0.7

完全免费，占用低(大概300MB内存)

### 先安装Docker

```
curl -fsSL https://get.docker.com | bash -s docker
#or curl -fsSL https://get.docker.com | bash -s docker --mirror Aliyun #阿里云镜像
```

### 下载镜像

```
wget https://github.com/qiuxiuya/Backup/raw/refs/heads/main/xdpanel/forwordpanel-1.0.7.tar
```

装载镜像

```
docker load < /root/forwordpanel-1.0.7.tar
```

### 查看镜像ID

```
docker images
```

### 启动镜像

比如id是 `ef796f049164`，则

```
 docker run --restart=always -d -p 8080:8080 ef796f049164
```

等待安装完毕，打开 http://你的ip:8080 即可

#### 默认账号密码为**`admin XIAOLIzz123`**

### 注意：添加的中转机请先安装iptables

```
apt install iptables -y
```
