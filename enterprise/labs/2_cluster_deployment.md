### use curl on the endpoint ./api/v2/cm/deployment
```
{
  "timestamp" : "2017-05-10T03:32:42.667Z",
  "clusters" : [ {
    "name" : "xiaohu-liu",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "1146093568"
          }, {
            "name" : "hive_metastore_server_max_message_size",
            "value" : "114609356"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "1707081728"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "1392194355"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "234"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-7-188"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_password"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-4b48582fb7deb4d024a640dd668a39d8",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-009c11f28418ae34a"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-5a3809689dc5512184bdee3b736e156e",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "6e1f32db-7c06-4e55-bd03-07f4f514350b"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-bce8c20cec27c2dbc2c9edb656438bbd",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "aa6b7d1e-228a-4f8f-8b32-8303e5ad401b"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-cbcc58a3b80b94c7765419a5d5859537",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "d0c2ad92-ed9e-4753-bb40-3665ee87c0b9"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-f180e8b2f2bf9a80be3bec9ce1065d02",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "7f0d8eda-d828-4937-ac15-a553f49fe3dc"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-5a3809689dc5512184bdee3b736e156e",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "6e1f32db-7c06-4e55-bd03-07f4f514350b"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bbzjm9f4qmvzoqq5ag2upk37g"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-bce8c20cec27c2dbc2c9edb656438bbd",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "aa6b7d1e-228a-4f8f-8b32-8303e5ad401b"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2zy7rei5ian0dvpma6n2zxv7a"
          } ]
        }
      }, {
        "name" : "hive-WEBHCAT-5a3809689dc5512184bdee3b736e156e",
        "type" : "WEBHCAT",
        "hostRef" : {
          "hostId" : "6e1f32db-7c06-4e55-bd03-07f4f514350b"
        },
        "config" : {
          "items" : [ {
            "name" : "hive_webhcat_secret_key",
            "value" : "UgsKnopirdKnLyn9r60Coc1V4Ar94w"
          }, {
            "name" : "role_jceks_password",
            "value" : "9zy0ueizd6lz1rnnrofplh7ts"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-4b48582fb7deb4d024a640dd668a39d8",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-009c11f28418ae34a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "l1fzolj5lb5lx9e7ze7ter4n"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-bce8c20cec27c2dbc2c9edb656438bbd",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "aa6b7d1e-228a-4f8f-8b32-8303e5ad401b"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1xz9c39amxnuz7gnqssk5ikpk"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-cbcc58a3b80b94c7765419a5d5859537",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "d0c2ad92-ed9e-4753-bb40-3665ee87c0b9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2966x74xa18t7vwz6nsdu2oqz"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-7-188"
        }, {
          "name" : "database_password",
          "value" : "huepassword"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-cbcc58a3b80b94c7765419a5d5859537"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-f180e8b2f2bf9a80be3bec9ce1065d02",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "7f0d8eda-d828-4937-ac15-a553f49fe3dc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cbeztebyydjryy0dirbypopqt"
          }, {
            "name" : "secret_key",
            "value" : "iDZXrIRlo3T05QoGP1eiNZtro4gqzi"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-7-188"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-cbcc58a3b80b94c7765419a5d5859537",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "d0c2ad92-ed9e-4753-bb40-3665ee87c0b9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cjkvqacrnjbnfum199puktzn"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "8"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "1024"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "1576"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "80"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "87vSdSpjf5dwzhhc9tIl2EBkSXf0a1"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-4b48582fb7deb4d024a640dd668a39d8",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "i-009c11f28418ae34a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7a316t5c84c2d9iop7tpr4ory"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-4b48582fb7deb4d024a640dd668a39d8",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-009c11f28418ae34a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ceai2t7nwjg60o3c66u9p52mw"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-bce8c20cec27c2dbc2c9edb656438bbd",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "aa6b7d1e-228a-4f8f-8b32-8303e5ad401b"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8y7evl4s1wdbedz3rgfowg4gw"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-cbcc58a3b80b94c7765419a5d5859537",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "d0c2ad92-ed9e-4753-bb40-3665ee87c0b9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1v1rnznsxhb32qc3q9fitib82"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-f180e8b2f2bf9a80be3bec9ce1065d02",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "7f0d8eda-d828-4937-ac15-a553f49fe3dc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6kfv9ih1fgvdtjgzw3fs6jifx"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-5a3809689dc5512184bdee3b736e156e",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "6e1f32db-7c06-4e55-bd03-07f4f514350b"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "103"
          }, {
            "name" : "role_jceks_password",
            "value" : "1ttv2sh88bqvqpazqh4mzmkqh"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "3170683699"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/dfs/jn"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "1146093568"
          }, {
            "name" : "role_config_suppression_namenode_java_heapsize_minimum_validator",
            "value" : "true"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "1146093568"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "UC3y9QVrf42UsjpfQwmmrRjo55f66p"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "7vNziBuSiz3iifLl2dImpDfgzl1KRM"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "bCrYBlNapotEUVwMFrBzQMESVdH5Pw"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "20"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-bce8c20cec27c2dbc2c9edb656438bbd",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "aa6b7d1e-228a-4f8f-8b32-8303e5ad401b"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-4b48582fb7deb4d024a640dd668a39d8",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-009c11f28418ae34a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "agfrroolfmwx62w1ksp1khbc5"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-bce8c20cec27c2dbc2c9edb656438bbd",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "aa6b7d1e-228a-4f8f-8b32-8303e5ad401b"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "c9yhx7lhxaog0wwhcamar589r"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-cbcc58a3b80b94c7765419a5d5859537",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "d0c2ad92-ed9e-4753-bb40-3665ee87c0b9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "enxbe70jhskwfh0371hpgdojj"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-f180e8b2f2bf9a80be3bec9ce1065d02",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "7f0d8eda-d828-4937-ac15-a553f49fe3dc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3zxz3ebzw1rgjddlc4us41dhs"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-5a3809689dc5512184bdee3b736e156e",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "6e1f32db-7c06-4e55-bd03-07f4f514350b"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3homv1d4ufwhvqpp0s8vdp2yw"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-f180e8b2f2bf9a80be3bec9ce1065d02",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "7f0d8eda-d828-4937-ac15-a553f49fe3dc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3to3bb1gll3nk9y7zpvmg8tt0"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-4b48582fb7deb4d024a640dd668a39d8",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "i-009c11f28418ae34a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cfiu7ufnli50lo0db4gpmklx2"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-cbcc58a3b80b94c7765419a5d5859537",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "d0c2ad92-ed9e-4753-bb40-3665ee87c0b9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7u19egfmf6pykj8redl5sc7cg"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-4b48582fb7deb4d024a640dd668a39d8",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-009c11f28418ae34a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ey2mpt11vrtvkjin942vc68cd"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-bce8c20cec27c2dbc2c9edb656438bbd",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "aa6b7d1e-228a-4f8f-8b32-8303e5ad401b"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7bpr167ej611crhso3x0sb83v"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-cbcc58a3b80b94c7765419a5d5859537",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "d0c2ad92-ed9e-4753-bb40-3665ee87c0b9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "700ilcad1whm7ypeybc36yb5n"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-5a3809689dc5512184bdee3b736e156e",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "6e1f32db-7c06-4e55-bd03-07f4f514350b"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "112"
          }, {
            "name" : "role_jceks_password",
            "value" : "a6mjm2qiuo23ls0j1k1kz7vad"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-f180e8b2f2bf9a80be3bec9ce1065d02",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "7f0d8eda-d828-4937-ac15-a553f49fe3dc"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "118"
          }, {
            "name" : "role_jceks_password",
            "value" : "9d9p3jq9jzyympyt6dnlfmcxt"
          } ]
        }
      }, {
        "name" : "hdfs-NFSGATEWAY-4b48582fb7deb4d024a640dd668a39d8",
        "type" : "NFSGATEWAY",
        "hostRef" : {
          "hostId" : "i-009c11f28418ae34a"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4pjaalrayvxnvsnz0vo9d1t7k"
          } ]
        }
      }, {
        "name" : "hdfs-NFSGATEWAY-5a3809689dc5512184bdee3b736e156e",
        "type" : "NFSGATEWAY",
        "hostRef" : {
          "hostId" : "6e1f32db-7c06-4e55-bd03-07f4f514350b"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6wjbxtsn9a6ik4drr02ugx1ob"
          } ]
        }
      }, {
        "name" : "hdfs-NFSGATEWAY-bce8c20cec27c2dbc2c9edb656438bbd",
        "type" : "NFSGATEWAY",
        "hostRef" : {
          "hostId" : "aa6b7d1e-228a-4f8f-8b32-8303e5ad401b"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "rcacv9omqu3jr79nw8waxq75"
          } ]
        }
      }, {
        "name" : "hdfs-NFSGATEWAY-cbcc58a3b80b94c7765419a5d5859537",
        "type" : "NFSGATEWAY",
        "hostRef" : {
          "hostId" : "d0c2ad92-ed9e-4753-bb40-3665ee87c0b9"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6dmq9yirkczgju8w2x0z66sb7"
          } ]
        }
      }, {
        "name" : "hdfs-NFSGATEWAY-f180e8b2f2bf9a80be3bec9ce1065d02",
        "type" : "NFSGATEWAY",
        "hostRef" : {
          "hostId" : "7f0d8eda-d828-4937-ac15-a553f49fe3dc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8d6iskwmebwtevkk81mu4wn4u"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "6e1f32db-7c06-4e55-bd03-07f4f514350b",
    "ipAddress" : "172.31.0.239",
    "hostname" : "ip-172-31-0-239",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-009c11f28418ae34a",
    "ipAddress" : "172.31.7.188",
    "hostname" : "ip-172-31-7-188",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "aa6b7d1e-228a-4f8f-8b32-8303e5ad401b",
    "ipAddress" : "172.31.7.206",
    "hostname" : "ip-172-31-7-206",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "d0c2ad92-ed9e-4753-bb40-3665ee87c0b9",
    "ipAddress" : "172.31.7.210",
    "hostname" : "ip-172-31-7-210",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "7f0d8eda-d828-4937-ac15-a553f49fe3dc",
    "ipAddress" : "172.31.8.15",
    "hostname" : "ip-172-31-8-15",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-ACTIVITYMONITOR-f180e8b2f2bf9a80be3bec9ce1065d02",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "2676e5d3e83decf7df63819e4f22e12dcc1b93f8b199eeb75bf02642650ae62e",
    "pwSalt" : 1836405318743126161,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-5a3809689dc5512184bdee3b736e156e",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "bbcaff918b751e5410008368e30c6152f90176708cabadac1a48e15efe6a086e",
    "pwSalt" : 6624657066930439049,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-5a3809689dc5512184bdee3b736e156e",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "c9dd24723fdfbffabf2eaf57071f9af0d8ff512248169c2e5f95caeadb051cba",
    "pwSalt" : -517704115823427010,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-4b48582fb7deb4d024a640dd668a39d8",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "f4fb3fa92ba06bd12f9de83a3b1e6fe079349a394d4cd889d64056c74bce1759",
    "pwSalt" : 961437022444269429,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-5a3809689dc5512184bdee3b736e156e",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "97ed585396ad82dcf49e17ff14a4d462216c72d0dded393e0fd1bf1e081aa172",
    "pwSalt" : 7244199771320467852,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "cbbeccc1ce21ccfacb95cff4e834e164d9fa1de9110eaad50790b44817038cc2",
    "pwSalt" : 3829454112955011153,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "7370301af8f297a4262f09c6c60af19fcf3c790f7d44f3ee33ec0f96a40514c0",
    "pwSalt" : 4961915522549562530,
    "pwLogin" : true
  }, {
    "name" : "xiaohu-liu",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "a3076a190ba9c59fff087c291671c2dd14a8a4b6fe3ddc6e10e653b06d5630f1",
    "pwSalt" : 4548583628694198139,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.9.2",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170330-1814",
    "gitHash" : "822da28bff818f57fc1bfc3eafe3a550300ef1b0",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "ACTIVITYMONITOR",
        "items" : [ {
          "name" : "firehose_database_host",
          "value" : "ip-172-31-7-188"
        }, {
          "name" : "firehose_database_name",
          "value" : "amon"
        }, {
          "name" : "firehose_database_password",
          "value" : "amon_password"
        }, {
          "name" : "firehose_database_user",
          "value" : "amon"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1490026496"
        }, {
          "name" : "role_config_suppression_firehose_non_java_memory_validator",
          "value" : "true"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-7-188"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_password"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1490026496"
        }, {
          "name" : "role_config_suppression_firehose_non_java_memory_validator",
          "value" : "true"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ACTIVITYMONITOR-f180e8b2f2bf9a80be3bec9ce1065d02",
      "type" : "ACTIVITYMONITOR",
      "hostRef" : {
        "hostId" : "7f0d8eda-d828-4937-ac15-a553f49fe3dc"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9x3mxam6ph2khtc875bnv368z"
        } ]
      }
    }, {
      "name" : "mgmt-ALERTPUBLISHER-5a3809689dc5512184bdee3b736e156e",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "6e1f32db-7c06-4e55-bd03-07f4f514350b"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "3k5e5tdjvb4l756e9pg5grdyc"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-5a3809689dc5512184bdee3b736e156e",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "6e1f32db-7c06-4e55-bd03-07f4f514350b"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "eeka3o9jgrv0haayuzxsk67a"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-5a3809689dc5512184bdee3b736e156e",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "6e1f32db-7c06-4e55-bd03-07f4f514350b"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "eya2qyz87nikgjgyrdcqkg2j5"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-4b48582fb7deb4d024a640dd668a39d8",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "i-009c11f28418ae34a"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "5c1pjz7qy8wc2kpdhy66x226y"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-5a3809689dc5512184bdee3b736e156e",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "6e1f32db-7c06-4e55-bd03-07f4f514350b"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9mw3paf14ce2irzurkumzwz7m"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/23/2012 5:30"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/,http://172.31.0.239/cdh5.11/,http://172.31.0.239/cdh5.8.4/"
    } ]
  }
}
```
