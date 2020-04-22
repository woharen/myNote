## Wget
Wget是一个从网络上自动下载文件的自由工具，支持通过HTTP、HTTPS、FTP三个最常见的TCP/IP协议下载，并可以使用HTTP代理。wget名称的由来是“World Wide Web”与“get”的结合。

### 安装命令
```shell
yum -y install wget
```
### 使用
```shell
wget [资源文件链接]
```

## PM2
pm2是一个进程管理工具,可以用它来管理你的node进程，并查看node进程的状态，当然也支持性能监控，进程守护，负载均衡等功能

### 安装命令
```shell
npm install -g pm2
```
### 使用

启动进程/应用 
```
pm2 start bin/www 或 pm2 start app.js
```

重命名进程/应用 
```
pm2 start app.js --name wb123
```

添加进程/应用 
```
watch pm2 start bin/www --watch
```

结束进程/应用 
```
pm2 stop www
```

结束所有进程/应用 
```
pm2 stop all
```

删除进程/应用 
```
pm2 delete www
```

删除所有进程/应用 
```
pm2 delete all
```

列出所有进程/应用 
```
pm2 list
```

查看某个进程/应用具体情况 
```
pm2 describe www
```

查看进程/应用的资源消耗情况 
```
pm2 monit
```

查看pm2的日志 
```
pm2 logs
```

若要查看某个进程/应用的日志,使用 
```
pm2 logs www
```

重新启动进程/应用 
```
pm2 restart www
```

重新启动所有进程/应用 
```
pm2 restart all
```

## unzip
### 安装命令
```shell
yum install -y unzip zip
```