## shadow socket script
execute ss.sh to create shadow socket servet-side
```
sh sh.sh 
```
## start shadow socket 
start shadow socket in background without output
```
nohup ssserver -c /etc/shadowsocks.json > /dev/null  &
```
