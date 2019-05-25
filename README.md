# ocserv
一个 CiscoCisco Anyconnect 多用户控制管理脚本

## 操作
### 下载 安装
```
wget -N --no-check-certificate https://raw.githubusercontent.com/lllvcs/ocserv/master/ocserv.sh && bash ocserv.sh
```
### 相关配置
```
sh_ver = 1.0.6
file = /usr/local/sbin/ocserv
conf_file = /etc/ocserv
conf = /etc/ocserv/ocserv.conf
passwd_file = /etc/ocserv/ocpasswd
log_file = /tmp/ocserv.log
ocserv_ver = 0.12.3
PID_FILE = /var/run/ocserv.pid
```

## 注意！
本脚本仅支持Debian和Ubuntu系统！