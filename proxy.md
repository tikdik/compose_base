##### docker代理设置
```
mkdir -p /etc/systemd/system/docker.service.d
vim /etc/systemd/system/docker.service.d/proxy.conf
```
```
[Service]
Environment="HTTP_PROXY=http://192.168.2.139:1080/"
Environment="HTTPS_PROXY=http://192.168.2.139:1080/"
```

#### wget下载代理
```
export http_proxy=http://192.168.2.139:1080
export https_proxy=http://192.168.2.139:1080
```
取消
```
unset http_proxy
unset https_proxy
```
