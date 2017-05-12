### The command and output for hdfs dfs -ls /user
```
[root@ip-172-31-7-7 yum.repos.d]# hdfs dfs -ls /user
Found 7 items
drwxr-xr-x   - hdfs   supergroup          0 2017-05-12 02:19 /user/chen
drwxrwxrwx   - mapred hadoop              0 2017-05-12 02:14 /user/history
drwxrwxr-t   - hive   hive                0 2017-05-12 02:14 /user/hive
drwxrwxr-x   - hue    hue                 0 2017-05-12 02:15 /user/hue
drwxrwxr-x   - impala impala              0 2017-05-12 02:15 /user/impala
drwxrwxr-x   - oozie  oozie               0 2017-05-12 02:15 /user/oozie
drwxr-xr-x   - hdfs   supergroup          0 2017-05-12 02:18 /user/zhou

```


### The command and output from the CM API call ../api/v14/hosts
```
[root@ip-172-31-7-7 yum.repos.d]# curl -u admin:admin -XGET 'http://localhost:7180/api/v14/hosts'
{
  "items" : [ {
    "hostId" : "0330ae07-7155-41d7-a2dc-f61be36cb453",
    "ipAddress" : "172.31.3.172",
    "hostname" : "ip-172-31-3-172",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-7-7:7180/cmf/hostRedirect/0330ae07-7155-41d7-a2dc-f61be36cb453",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 8,
    "numPhysicalCores" : 8,
    "totalPhysMemBytes" : 15739797504
  }, {
    "hostId" : "010852de-c175-449c-9f82-ea84ea5b6369",
    "ipAddress" : "172.31.4.25",
    "hostname" : "ip-172-31-4-25",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-7-7:7180/cmf/hostRedirect/010852de-c175-449c-9f82-ea84ea5b6369",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 8,
    "numPhysicalCores" : 8,
    "totalPhysMemBytes" : 15739797504
  }, {
    "hostId" : "edf60441-4525-4057-8d4c-1a33d1ec77af",
    "ipAddress" : "172.31.7.7",
    "hostname" : "ip-172-31-7-7",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-7-7:7180/cmf/hostRedirect/edf60441-4525-4057-8d4c-1a33d1ec77af",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 8,
    "numPhysicalCores" : 8,
    "totalPhysMemBytes" : 15739797504
  }, {
    "hostId" : "4fdcd692-2e6b-4d59-a23d-18319a841e5b",
    "ipAddress" : "172.31.8.23",
    "hostname" : "ip-172-31-8-23",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-7-7:7180/cmf/hostRedirect/4fdcd692-2e6b-4d59-a23d-18319a841e5b",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 8,
    "numPhysicalCores" : 8,
    "totalPhysMemBytes" : 15739797504
  }, {
    "hostId" : "66e2184e-37f9-4942-98c0-ade0d7153d2e",
    "ipAddress" : "172.31.8.253",
    "hostname" : "ip-172-31-8-253",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-7-7:7180/cmf/hostRedirect/66e2184e-37f9-4942-98c0-ade0d7153d2e",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 8,
    "numPhysicalCores" : 8,
    "totalPhysMemBytes" : 15739797504
  } ]
}
```
### The command and output from the CM API call ../api/v6/clusters/<githubName>/services
```
[root@ip-172-31-7-7 yum.repos.d]# curl -u admin:admin -XGET 'http://localhost:7180/api/v6/clusters/xiaohu-liu/services'
{
  "items" : [ {
    "name" : "hive",
    "type" : "HIVE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-7-7:7180/cmf/serviceRedirect/hive",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HIVE_HIVEMETASTORES_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HIVE_HIVESERVER2S_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HIVE_WEBHCATS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hive"
  }, {
    "name" : "zookeeper",
    "type" : "ZOOKEEPER",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-7-7:7180/cmf/serviceRedirect/zookeeper",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "ZOOKEEPER_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "ZooKeeper"
  }, {
    "name" : "hue",
    "type" : "HUE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-7-7:7180/cmf/serviceRedirect/hue",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HUE_HUE_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hue"
  }, {
    "name" : "oozie",
    "type" : "OOZIE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-7-7:7180/cmf/serviceRedirect/oozie",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Oozie"
  }, {
    "name" : "impala",
    "type" : "IMPALA",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-7-7:7180/cmf/serviceRedirect/impala",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "IMPALA_ASSIGNMENT_LOCALITY",
      "summary" : "DISABLED"
    }, {
      "name" : "IMPALA_CATALOGSERVER_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "IMPALA_IMPALADS_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "IMPALA_STATESTORE_HEALTH",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Impala"
  }, {
    "name" : "yarn",
    "type" : "YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-7-7:7180/cmf/serviceRedirect/yarn",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "YARN_JOBHISTORY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_NODE_MANAGERS_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_RESOURCEMANAGERS_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_USAGE_AGGREGATION_HEALTH",
      "summary" : "DISABLED"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "YARN (MR2 Included)"
  }, {
    "name" : "hdfs",
    "type" : "HDFS",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-7-7:7180/cmf/serviceRedirect/hdfs",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_DATA_NODES_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_FREE_SPACE_REMAINING",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_HA_NAMENODE_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_MISSING_BLOCKS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HDFS"
  } ]
}
```

