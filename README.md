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

## 其他
如遇到ping通但无法上网的情况，请尝试如下操作
```
添加iptables转发
iptables -A FORWARD -d 10.250.250.0/24 -j ACCEPT
然后打开
/etc/sysctl.conf
修改
net.ipv4.ip_forward = 1
修改好后运行
sysctl -p /etc/sysctl.conf
```