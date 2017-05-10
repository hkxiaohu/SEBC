### curl statement that stop Hive service
```
curl -u "xiaohu-liu:cloudera" -XPOST 'http://localhost:7180/api/v12/clusters/xiaohu-liu/servces/hive/commands/stop'
{
  "id" : 693,
  "name" : "Stop",
  "startTime" : "2017-05-10T03:39:18.731Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

### check the status of the previous stop command
```
[root@ip-172-31-7-188 tmp]# curl -u "xiaohu-liu:cloudera"  'http://localhost:7180/api/v12/commands/693'
{
  "id" : 693,
  "name" : "Stop",
  "startTime" : "2017-05-10T03:39:18.731Z",
  "endTime" : "2017-05-10T03:39:22.253Z",
  "active" : false,
  "success" : true,
  "resultMessage" : "Successfully stopped service.",
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  },
  "children" : {
    "items" : [ {
      "id" : 694,
      "name" : "Stop",
      "startTime" : "2017-05-10T03:39:18.734Z",
      "endTime" : "2017-05-10T03:39:22.253Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-WEBHCAT-5a3809689dc5512184bdee3b736e156e"
      }
    }, {
      "id" : 695,
      "name" : "Stop",
      "startTime" : "2017-05-10T03:39:18.737Z",
      "endTime" : "2017-05-10T03:39:20.826Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-HIVESERVER2-bce8c20cec27c2dbc2c9edb656438bbd"
      }
    }, {
      "id" : 696,
      "name" : "Stop",
      "startTime" : "2017-05-10T03:39:18.739Z",
      "endTime" : "2017-05-10T03:39:22.244Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-HIVEMETASTORE-5a3809689dc5512184bdee3b736e156e"
      }
    } ]
  },
  "canRetry" : false
}
```

```
### curl statement that start Hive service
[root@ip-172-31-7-188 tmp]# curl -u "xiaohu-liu:cloudera" -XPOST 'http://localhost:7180/api/v12/clusters/xiaohu-liu/services/hive/commands/start'
{
  "id" : 698,
  "name" : "Start",
  "startTime" : "2017-05-10T03:47:02.444Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

### curl statement to check the current state of Hive service
```
[root@ip-172-31-7-188 tmp]# curl -u "xiaohu-liu:cloudera"  'http://localhost:7180/api/v12/clusters/xiaohu-liu/services/hive'
{
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://ip-172-31-7-188:7180/cmf/serviceRedirect/hive",
  "roleInstancesUrl" : "http://ip-172-31-7-188:7180/cmf/serviceRedirect/hive/instances",
  "serviceState" : "STARTED",
  "healthSummary" : "GOOD",
  "healthChecks" : [ {
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  }, {
    "name" : "HIVE_HIVESERVER2S_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  }, {
    "name" : "HIVE_WEBHCATS_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  } ],
  "configStalenessStatus" : "FRESH",
  "clientConfigStalenessStatus" : "STALE",
  "maintenanceMode" : false,
  "maintenanceOwners" : [ ],
  "displayName" : "Hive",
  "entityStatus" : "GOOD_HEALTH"
}
```[root@ip-172-31-7-188 tmp]# curl -u "xiaohu-liu:cloudera"  'http://localhost:7180/api/v12/clusters/xiaohu-liu/services/hive'
{
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://ip-172-31-7-188:7180/cmf/serviceRedirect/hive",
  "roleInstancesUrl" : "http://ip-172-31-7-188:7180/cmf/serviceRedirect/hive/instances",
  "serviceState" : "STARTED",
  "healthSummary" : "GOOD",
  "healthChecks" : [ {
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  }, {
    "name" : "HIVE_HIVESERVER2S_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  }, {
    "name" : "HIVE_WEBHCATS_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  } ],
  "configStalenessStatus" : "FRESH",
  "clientConfigStalenessStatus" : "STALE",
  "maintenanceMode" : false,
  "maintenanceOwners" : [ ],
  "displayName" : "Hive",
  "entityStatus" : "GOOD_HEALTH"
}
