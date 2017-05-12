### The hostname of your database server
```
[root@ip-172-31-4-25 ~]# hostname
ip-172-31-4-25
```

### The command and output for showing the database server version
```
[root@ip-172-31-4-25 ~]# mysql --version
mysql  Ver 14.14 Distrib 5.6.36, for Linux (x86_64) using  EditLine wrapper
```
### The command and output for listing the databases created above
```
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| amon               |
| hive               |
| hue                |
| mysql              |
| nav                |
| navms              |
| oozie              |
| performance_schema |
| rman               |
| sentry             |
+--------------------+
11 rows in set (0.00 sec)

```
