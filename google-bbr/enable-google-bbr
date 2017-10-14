## enable google bbr
### step 0
	upgrade linux kernel >= 4.9
### step 1
```
echo "net.core.default_qdisc=fq" >> /etc/sysctl.conf
echo "net.ipv4.tcp_congestion_control=bbr" >> /etc/sysctl.conf
```
### step 2
```
sysctl -p
```
