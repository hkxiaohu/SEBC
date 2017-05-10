### Upgrade Cloudera Manager from version 5.9  to 5.11

### Report the latest available version of the API
```
[root@ip-172-31-7-188 yum.repos.d]# curl -u "xiaohu-liu:cloudera" -XGET 'http://localhost:7180/api/version'
v16
```

### Report the CM version
```
[root@ip-172-31-7-188 yum.repos.d]# curl -u xiaohu-liu:cloudera 'http://localhost:7180/api/v16/cm/version'
{
  "version" : "5.11.0",
  "buildUser" : "jenkins",
  "buildTimestamp" : "20170412-1249",
  "gitHash" : "70cb1442626406432a6e7af5bdf206a384ca3f98",
  "snapshot" : false
}
```

### List all CM users
```
[root@ip-172-31-7-188 yum.repos.d]# curl -u xiaohu-liu:cloudera 'http://localhost:7180/api/v16/users'
{
  "items" : [ {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ]
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ]
  }, {
    "name" : "xiaohu-liu",
    "roles" : [ "ROLE_ADMIN" ]
  } ]
}
```

### Report the database server in use by CM
```
[root@ip-172-31-7-188 yum.repos.d]# curl -u xiaohu-liu:cloudera -XGET 'http://localhost:7180/api/v16/cm/scmDbInfo'
{
  "scmDbType" : "MYSQL",
  "embeddedDbUsed" : false
}
```
