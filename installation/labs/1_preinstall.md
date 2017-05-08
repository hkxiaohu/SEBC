Check vm.swappiness on all your nodes Set the value to 1 if necessary
```
[root@ip-172-31-7-188 .ssh]# sysctl vm.swappiness
vm.swappiness = 1
```

Show the mount attributes of your volume(s)
```
[root@ip-172-31-7-188 .ssh]# cat /proc/mounts | grep ext4
/dev/xvde / ext4 rw,seclabel,relatime,barrier=1,data=ordered 0 0'
```
If you have ext-based volumes, list the reserve space setting
```
[root@ip-172-31-7-188 .ssh]# tune2fs -l /dev/xvde | grep "Reserved block count"
Reserved block count:     393145
```

Disable transparent hugepage support
```
[root@ip-172-31-7-188 .ssh]# grep -i HugePages_Total /proc/meminfo
HugePages_Total:       0
```

List your network interface configuration
```
[root@ip-172-31-7-188 .ssh]# ifconfig
eth0      Link encap:Ethernet  HWaddr 0A:AD:8C:12:85:F8  
          inet addr:172.31.7.188  Bcast:172.31.15.255  Mask:255.255.240.0
          inet6 addr: fe80::8ad:8cff:fe12:85f8/64 Scope:Link
          UP BROADCAST RUNNING MULTICAST  MTU:9001  Metric:1
          RX packets:34992 errors:0 dropped:0 overruns:0 frame:0
          TX packets:8243 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1000 
          RX bytes:47881155 (45.6 MiB)  TX bytes:861223 (841.0 KiB)
          Interrupt:24 

lo        Link encap:Local Loopback  
          inet addr:127.0.0.1  Mask:255.0.0.0
          inet6 addr: ::1/128 Scope:Host
          UP LOOPBACK RUNNING  MTU:16436  Metric:1
          RX packets:4 errors:0 dropped:0 overruns:0 frame:0
          TX packets:4 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:0 
          RX bytes:336 (336.0 b)  TX bytes:336 (336.0 b)
```

Show that forward and reverse host lookups are correctly resolved
```
[root@ip-172-31-7-188 .ssh]# getent hosts
127.0.0.1       localhost.localdomain localhost
127.0.0.1       localhost6.localdomain6 localhost6
172.31.7.188    ip-172-31-7-188 cdh1
172.31.8.15     ip-172-31-8-15 cdh2
172.31.7.210    ip-172-31-7-210 cdh3
172.31.7.206    ip-172-31-7-206 cdh4
172.31.0.239    ip-172-31-0-239 cdh5
```

Show the nscd service is running
```
[root@ip-172-31-7-188 .ssh]# service nscd status
nscd (pid 1236) is running...
```

Show the ntpd service is running
```
[root@ip-172-31-7-188 .ssh]# service ntpd status
ntpd (pid  1277) is running...
```
