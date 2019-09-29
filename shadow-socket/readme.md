## shadow socket script
execute ss.sh to create shadow socket servet-side
```
sh sh.sh 
```
## start shadow socket 

## Jobs
Start shadow socket in background without output
```
nohup ssserver -c /etc/shadowsocks.json > /dev/null  &
```

### Daemon
```
ssserver -c /etc/shadowsocks.json -d start
```

### Alter Port

If you change port from config file `/etc/shadowsocks.json`, you must open port for firewall.
```
firewall-cmd --permanent --add-port=XXX/tcp // xxx is your target port number.
```
