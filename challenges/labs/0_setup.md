### List the cloud provider you are using (AWS, GCE, Azure, other)
```
AWS
```

### List your instances by their IP address and DNS name
```
172.31.4.25     ip-172-31-4-25 cdh2
172.31.7.7      ip-172-31-7-7 cdh1
172.31.8.23     ip-172-31-8-23 cdh3
172.31.8.253    ip-172-31-8-253 cdh4
172.31.3.172    ip-172-31-3-172 cdh5

```

### List the Linux release you are using
```
CentOS release 6.5 (Final)
```

### List the file system capacity for the first node
```
[root@ip-172-31-4-25 ~]# df -Th
Filesystem     Type   Size  Used Avail Use% Mounted on
/dev/xvde      ext4    30G  1.2G   27G   4% /
tmpfs          tmpfs  7.4G     0  7.4G   0% /dev/shm

```

### List the command and output for yum repolist enabled
```
repo id                                               repo name                                                    status
base                                                  CentOS-6 - Base                                              6,706
cloudera-manager                                      Cloudera Manager, Version 5.11.0                                 7
extras                                                CentOS-6 - Extras                                               64
mysql-connectors-community                            MySQL Connectors Community                                      36
mysql-tools-community                                 MySQL Tools Community                                           47
mysql55-community                                     MySQL 5.5 Community Server                                     373
updates                                               CentOS-6 - Updates                                             270

```
### List the /etc/passwd entries for zhou and chen
```
[root@ip-172-31-7-7 ~]# grep -E 'zhou|chen' /etc/passwd
zhou:x:2800:2800::/home/zhou:/bin/bash
chen:x:2900:2900::/home/chen:/bin/bash
```

### List the /etc/group entries for shanghai and beijing
```
[root@ip-172-31-7-7 ~]# grep -E 'shanghai|beijing' /etc/group
shanghai:x:2901:chen
beijing:x:2902:zhou

```
