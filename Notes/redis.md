# redis CentOS7

此安装过程，基于GUI桌面，不是最小化安装

## 安装

- 使用root权限,下面操作使用管理员权限

 ```bash
    su
```
    输入密码
- 使用yum安装

```bash
    yum -y install redis
```

- 安装好之后启动Redis服务

```bash
    systemctl start redis
```
- 配置config

    另外为了可以使 Redis 能被远程连接，需要修改配置文件，路径为 /etc/redis.conf。

```bash
    vim /etc/redis.conf
```
    1.修改这一行
    bing 127.0.0.1 
    例：
    # bing 127.0.0.1
    或：
    bind 0.0.0.0

    2.推荐按设置密码
    requirepass foobared
    例：
    requirepass password

    3. 配置后台运行
    daemonize yes

    4.关闭保护模式
    protected-mode no

- 重启Redis服务

```bash
    systemctl restart redis
```

## 其他操作

### 启动等操作

```bash
# 启动
systemctl start redis

# 查看状态
systemctl status redis

# 停止
systemctl stop redis

# 重启
systemctl restart redis
```

### 防火墙

主机不能连接虚拟机的redis，关闭防火墙
```bash
# 查看防火墙状态
systemctl status firewalld.service

# 开启防火墙
systemctl start firewalld.service

# 关闭防火墙
systemctl stop firewalld.service

# 禁用防火墙服务
systemctl disable firewalld.service
```