## import key
```
rpm --import https://www.elrepo.org/RPM-GPG-KEY-elrepo.org
```
## install yum
```
rpm -Uvh http://www.elrepo.org/elrepo-release-7.0-2.el7.elrepo.noarch.rpm
```
## install kernel
```
yum --enablerepo=elrepo-kernel install  kernel-ml-devel kernel-ml
```
## change startup kernel
### list kernel
```
awk -F\' '$1=="menuentry " {print $2}' /etc/grub2.cfg
```
### change kernel
```
grub2-set-default 0
```
## restart
```
reboot
```
## show kernel 
```
uname -r
```
## del old kernel
```
yum remove kernel
```
## note
   execute command with root
## reference
	[Come from](http://blog.csdn.net/silentwolfyh/article/details/52047780)
