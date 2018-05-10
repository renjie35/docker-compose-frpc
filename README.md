# Zookeeper

## 一.下载&导入&运行
github镜像下载地址：

```
wget --no-check-certificate https://github.com/clangcn/frp-docker/raw/master/frps-docker/frps-docker.tar
```

导入命令:

```
docker load < frps-docker.tar
```

运行命令:

```
docker-compose up -d
```
## 二.变量说明

|变量名|默认值|描述|
|:-:|:-:|:-:| 
|set_bind_port|5443|frps服务端口，用于客户端连接|
|set_vhost_http_port|80|默认http穿透的端口。|
|set_vhost_https_port|	443|默认https穿透服务的端口|
|set_privilege_token|password|frps的特权密码，用于客户端连接|
|set_max_pool_count	|50|最大连接池数，貌似不用这个了|
|str_log_level|info|日志等级，可选项：debug, info, warn, error|
|set_log_max_days|3|日志保存天数，默认保存3天的|