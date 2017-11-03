[root@ip-172-31-47-134 jdk1.7.0_67-cloudera]# hdfs dfs -ls /user
Found 9 items
drwxr-xr-x   - admin    admin               0 2017-11-03 05:48 /user/admin
drwxr-xr-x   - frankola frankola            0 2017-11-03 05:49 /user/frankola
drwxr-xr-x   - hdfs     supergroup          0 2017-11-03 05:48 /user/hdfs
drwxrwxrwx   - mapred   hadoop              0 2017-11-03 05:43 /user/history
drwxrwxr-t   - hive     hive                0 2017-11-03 05:45 /user/hive
drwxrwxr-x   - hue      hue                 0 2017-11-03 05:45 /user/hue
drwxrwxr-x   - oozie    oozie               0 2017-11-03 05:46 /user/oozie
drwxr-xr-x   - reilly   reilly              0 2017-11-03 05:49 /user/reilly
drwxr-x--x   - spark    spark               0 2017-11-03 05:44 /user/spark



[root@ip-172-31-47-134 jdk1.7.0_67-cloudera]# curl -u admin:admin 'http://172.31.47.134:7180/api/v14/hosts'
{
  "items" : [ {
    "hostId" : "9ffe1030-ce20-42f1-9b4d-33e80b1b1ce0",
    "ipAddress" : "172.31.39.17",
    "hostname" : "ip-172-31-39-17.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/hostRedirect/9ffe1030-ce20-42f1-9b4d-33e80b1b1ce0",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332311040
  }, {
    "hostId" : "49b066cc-69e7-4a85-ac3d-2173c6666aab",
    "ipAddress" : "172.31.39.184",
    "hostname" : "ip-172-31-39-184.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/hostRedirect/49b066cc-69e7-4a85-ac3d-2173c6666aab",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332311040
  }, {
    "hostId" : "a1960418-6170-4067-834f-1d3460ced1b1",
    "ipAddress" : "172.31.44.186",
    "hostname" : "ip-172-31-44-186.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/hostRedirect/a1960418-6170-4067-834f-1d3460ced1b1",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332311040
  }, {
    "hostId" : "d71ee147-1b3b-4eeb-b627-a75820f0262d",
    "ipAddress" : "172.31.45.113",
    "hostname" : "ip-172-31-45-113.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/hostRedirect/d71ee147-1b3b-4eeb-b627-a75820f0262d",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332311040
  }, {
    "hostId" : "905a41f4-92ce-4890-9f91-8da8a4ad75b5",
    "ipAddress" : "172.31.47.134",
    "hostname" : "ip-172-31-47-134.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/hostRedirect/905a41f4-92ce-4890-9f91-8da8a4ad75b5",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332311040
  } ]





[root@ip-172-31-47-134 jdk1.7.0_67-cloudera]# curl -u admin:admin 'http://172.31.47.134:7180/api/v11/clusters/smarrone/services'
{
  "items" : [ {
    "name" : "hive",
    "type" : "HIVE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hive",
    "roleInstancesUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hive/instances",
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
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hive",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "zookeeper",
    "type" : "ZOOKEEPER",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/zookeeper",
    "roleInstancesUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/zookeeper/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "ZOOKEEPER_CANARY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "ZooKeeper",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hue",
    "type" : "HUE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hue",
    "roleInstancesUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hue/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HUE_HUE_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hue",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "oozie",
    "type" : "OOZIE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/oozie",
    "roleInstancesUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/oozie/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Oozie",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "yarn",
    "type" : "YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/yarn",
    "roleInstancesUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/yarn/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "YARN_JOBHISTORY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "YARN_NODE_MANAGERS_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "YARN_RESOURCEMANAGERS_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "YARN_USAGE_AGGREGATION_HEALTH",
      "summary" : "DISABLED",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "YARN (MR2 Included)",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "spark_on_yarn",
    "type" : "SPARK_ON_YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/spark_on_yarn",
    "roleInstancesUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/spark_on_yarn/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Spark",
    "entityStatus" : "GOOD_HEALTH"
  }, {
    "name" : "hdfs",
    "type" : "HDFS",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hdfs",
    "roleInstancesUrl" : "http://ip-172-31-47-134.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hdfs/instances",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_CANARY_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_DATA_NODES_HEALTHY",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_FREE_SPACE_REMAINING",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_HA_NAMENODE_HEALTH",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_MISSING_BLOCKS",
      "summary" : "GOOD",
      "suppressed" : false
    }, {
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
      "summary" : "GOOD",
      "suppressed" : false
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HDFS",
    "entityStatus" : "GOOD_HEALTH"
  } ]
}







[root@ip-172-31-47-134 jdk1.7.0_67-cloudera]# curl -u admin:admin "http://172.31.47.134:7180/api/v9/cm/deployment"
{
  "timestamp" : "2017-11-03T09:52:58.633Z",
  "clusters" : [ {
    "name" : "cluster",
    "displayName" : "smarrone",
    "version" : "CDH5",
    "fullVersion" : "5.8.5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-44-186.eu-central-1.compute.internal"
        }, {
          "name" : "hive_metastore_database_name",
          "value" : "hive"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_password"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "spark_on_yarn_service",
          "value" : "spark_on_yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-386d77ab753d80c97f9872b4dda6d43c",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "9ffe1030-ce20-42f1-9b4d-33e80b1b1ce0"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-3a872f1d47cf4d5711dcb5e260a0548a",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "905a41f4-92ce-4890-9f91-8da8a4ad75b5"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-52b05a4835689b61f2ad675eb1e77a3e",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "49b066cc-69e7-4a85-ac3d-2173c6666aab"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-6f89dc7bf1c68f5e21a360a65022ade6",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "d71ee147-1b3b-4eeb-b627-a75820f0262d"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-830c8cefc44cadd38a1ce6397cebca4a",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "a1960418-6170-4067-834f-1d3460ced1b1"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-HIVEMETASTORE-830c8cefc44cadd38a1ce6397cebca4a",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "a1960418-6170-4067-834f-1d3460ced1b1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8v09f6syoke2v0bs92tp4umrj"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVEMETASTORE-BASE"
        }
      }, {
        "name" : "hive-HIVESERVER2-386d77ab753d80c97f9872b4dda6d43c",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "9ffe1030-ce20-42f1-9b4d-33e80b1b1ce0"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "d4v7easka6mcj6yxjq6fwviyc"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVESERVER2-BASE"
        }
      }, {
        "name" : "hive-HIVESERVER2-830c8cefc44cadd38a1ce6397cebca4a",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "a1960418-6170-4067-834f-1d3460ced1b1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8cffx0fvbvi6ub30rn68ccm9u"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVESERVER2-1"
        }
      } ],
      "displayName" : "Hive",
      "roleConfigGroups" : [ {
        "name" : "hive-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-BASE",
        "displayName" : "Hive Metastore Server Default Group",
        "roleType" : "HIVEMETASTORE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "1330642944"
          }, {
            "name" : "hive_metastore_server_max_message_size",
            "value" : "133064294"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-1",
        "displayName" : "HiveServer2 Group 1",
        "roleType" : "HIVESERVER2",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "1330642944"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "1012504985"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "170"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-BASE",
        "displayName" : "HiveServer2 Default Group",
        "roleType" : "HIVESERVER2",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "1552941056"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "1012504985"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "170"
          } ]
        }
      }, {
        "name" : "hive-WEBHCAT-BASE",
        "displayName" : "WebHCat Server Default Group",
        "roleType" : "WEBHCAT",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ ]
        }
      } ],
      "replicationSchedules" : [ ]
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-386d77ab753d80c97f9872b4dda6d43c",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "9ffe1030-ce20-42f1-9b4d-33e80b1b1ce0"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "f0smve0vem002wx2bnxwvwbxq"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-52b05a4835689b61f2ad675eb1e77a3e",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "49b066cc-69e7-4a85-ac3d-2173c6666aab"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "a0gleqv6bjt5wv3ha0sbf1llx"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-6f89dc7bf1c68f5e21a360a65022ade6",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "d71ee147-1b3b-4eeb-b627-a75820f0262d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "akyaza62gddenlr8zgnbhe46f"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      } ],
      "displayName" : "ZooKeeper",
      "roleConfigGroups" : [ {
        "name" : "zookeeper-SERVER-BASE",
        "displayName" : "Server Default Group",
        "roleType" : "SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "zookeeper"
        },
        "config" : {
          "items" : [ ]
        }
      } ]
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-44-186.eu-central-1.compute.internal"
        }, {
          "name" : "database_password",
          "value" : "hue_password"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-830c8cefc44cadd38a1ce6397cebca4a"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-830c8cefc44cadd38a1ce6397cebca4a",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "a1960418-6170-4067-834f-1d3460ced1b1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1mxn8w04wwauk0qg5eldqte5g"
          }, {
            "name" : "secret_key",
            "value" : "6aPpWso0vAA3pLN8emobvD8NKQ2NZW"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hue-HUE_SERVER-BASE"
        }
      } ],
      "displayName" : "Hue",
      "roleConfigGroups" : [ {
        "name" : "hue-HUE_LOAD_BALANCER-BASE",
        "displayName" : "Load Balancer Default Group",
        "roleType" : "HUE_LOAD_BALANCER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hue-HUE_SERVER-BASE",
        "displayName" : "Hue Server Default Group",
        "roleType" : "HUE_SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hue-KT_RENEWER-BASE",
        "displayName" : "Kerberos Ticket Renewer Default Group",
        "roleType" : "KT_RENEWER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      } ]
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "spark_on_yarn_service",
          "value" : "spark_on_yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-830c8cefc44cadd38a1ce6397cebca4a",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "a1960418-6170-4067-834f-1d3460ced1b1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7830saphhhqr03xtpir50nncv"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "oozie-OOZIE_SERVER-BASE"
        }
      } ],
      "displayName" : "Oozie",
      "roleConfigGroups" : [ {
        "name" : "oozie-OOZIE_SERVER-BASE",
        "displayName" : "Oozie Server Default Group",
        "roleType" : "OOZIE_SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "oozie"
        },
        "config" : {
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-44-186.eu-central-1.compute.internal"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie_password"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          } ]
        }
      } ]
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "WEpJzGZjG32bNYWV8QzCXiBTpF8i8d"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-6f89dc7bf1c68f5e21a360a65022ade6",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "d71ee147-1b3b-4eeb-b627-a75820f0262d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1e2rdcrxqjbbu9fai2mr0iocd"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-JOBHISTORY-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-386d77ab753d80c97f9872b4dda6d43c",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "9ffe1030-ce20-42f1-9b4d-33e80b1b1ce0"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "axx3oct7zmy7zb2e2k93qtcqe"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-1"
        }
      }, {
        "name" : "yarn-NODEMANAGER-3a872f1d47cf4d5711dcb5e260a0548a",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "905a41f4-92ce-4890-9f91-8da8a4ad75b5"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2occ6bdewibv4b35wmoykf64i"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-52b05a4835689b61f2ad675eb1e77a3e",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "49b066cc-69e7-4a85-ac3d-2173c6666aab"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ciirxw1yezcfe953io8edc33"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-3"
        }
      }, {
        "name" : "yarn-NODEMANAGER-6f89dc7bf1c68f5e21a360a65022ade6",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "d71ee147-1b3b-4eeb-b627-a75820f0262d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "35owv872ykj5xc78t0eebwzmv"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-2"
        }
      }, {
        "name" : "yarn-NODEMANAGER-830c8cefc44cadd38a1ce6397cebca4a",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "a1960418-6170-4067-834f-1d3460ced1b1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "38o88yehq4z2sk2npsj315yu6"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-4"
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-52b05a4835689b61f2ad675eb1e77a3e",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "49b066cc-69e7-4a85-ac3d-2173c6666aab"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "65"
          }, {
            "name" : "role_jceks_password",
            "value" : "8l411f7gtluj3nluivztwfkc4"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-RESOURCEMANAGER-BASE"
        }
      } ],
      "displayName" : "YARN (MR2 Included)",
      "roleConfigGroups" : [ {
        "name" : "yarn-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "10"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "yarn-JOBHISTORY-BASE",
        "displayName" : "JobHistory Server Default Group",
        "roleType" : "JOBHISTORY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-1",
        "displayName" : "NodeManager Group 1",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
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
            "value" : "1926"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-2",
        "displayName" : "NodeManager Group 2",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
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
            "value" : "2520"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-3",
        "displayName" : "NodeManager Group 3",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
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
            "value" : "2124"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-4",
        "displayName" : "NodeManager Group 4",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
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
            "value" : "1650"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-BASE",
        "displayName" : "NodeManager Default Group",
        "roleType" : "NODEMANAGER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "node_manager_java_heapsize",
            "value" : "916455424"
          }, {
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
            "value" : "1136"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-BASE",
        "displayName" : "ResourceManager Default Group",
        "roleType" : "RESOURCEMANAGER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "2520"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "4"
          } ]
        }
      } ]
    }, {
      "name" : "spark_on_yarn",
      "type" : "SPARK_ON_YARN",
      "config" : {
        "items" : [ {
          "name" : "yarn_service",
          "value" : "yarn"
        } ]
      },
      "roles" : [ {
        "name" : "spar40365358-SPARK_YARN_HISTORY_SERVER-830c8cefc44cadd38a1ce6397",
        "type" : "SPARK_YARN_HISTORY_SERVER",
        "hostRef" : {
          "hostId" : "a1960418-6170-4067-834f-1d3460ced1b1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2x3h76b1orr68sg52g9s5kgvi"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "spark_on_yarn-SPARK_YARN_HISTORY_SERVER-BASE"
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-386d77ab753d80c97f9872b4dda6d43c",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "9ffe1030-ce20-42f1-9b4d-33e80b1b1ce0"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "spark_on_yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-3a872f1d47cf4d5711dcb5e260a0548a",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "905a41f4-92ce-4890-9f91-8da8a4ad75b5"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "spark_on_yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-52b05a4835689b61f2ad675eb1e77a3e",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "49b066cc-69e7-4a85-ac3d-2173c6666aab"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "spark_on_yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-6f89dc7bf1c68f5e21a360a65022ade6",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "d71ee147-1b3b-4eeb-b627-a75820f0262d"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "spark_on_yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "spark_on_yarn-GATEWAY-830c8cefc44cadd38a1ce6397cebca4a",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "a1960418-6170-4067-834f-1d3460ced1b1"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "spark_on_yarn-GATEWAY-BASE"
        }
      } ],
      "displayName" : "Spark",
      "roleConfigGroups" : [ {
        "name" : "spark_on_yarn-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "spark_on_yarn"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "spark_on_yarn-SPARK_YARN_HISTORY_SERVER-BASE",
        "displayName" : "History Server Default Group",
        "roleType" : "SPARK_YARN_HISTORY_SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "spark_on_yarn"
        },
        "config" : {
          "items" : [ ]
        }
      } ]
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "DkwSXPhlGmDDT95bvmymRUcarKkqA1"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "2SZM6RxfIaSpBpxVNuIVfbk0x4EjPG"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "gQxd0P1Izxpjoibtu6ssGuanJ8FVCH"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-6f89dc7bf1c68f5e21a360a65022ade6",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "d71ee147-1b3b-4eeb-b627-a75820f0262d"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-BALANCER-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-386d77ab753d80c97f9872b4dda6d43c",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "9ffe1030-ce20-42f1-9b4d-33e80b1b1ce0"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7j017ugg21btnwhpr43yzbm00"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-3a872f1d47cf4d5711dcb5e260a0548a",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "905a41f4-92ce-4890-9f91-8da8a4ad75b5"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "edfp2rcueakn8ztdl9ssf3vxo"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-4"
        }
      }, {
        "name" : "hdfs-DATANODE-52b05a4835689b61f2ad675eb1e77a3e",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "49b066cc-69e7-4a85-ac3d-2173c6666aab"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7bl2a89emdhvohr2f3ounzf4n"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-2"
        }
      }, {
        "name" : "hdfs-DATANODE-6f89dc7bf1c68f5e21a360a65022ade6",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "d71ee147-1b3b-4eeb-b627-a75820f0262d"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5jejxtxk2b08kvbv3vfbuar3d"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-1"
        }
      }, {
        "name" : "hdfs-DATANODE-830c8cefc44cadd38a1ce6397cebca4a",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "a1960418-6170-4067-834f-1d3460ced1b1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "15lqkhs6txq3ecn6txgi0kggz"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-3"
        }
      }, {
        "name" : "hdfs-HTTPFS-830c8cefc44cadd38a1ce6397cebca4a",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "a1960418-6170-4067-834f-1d3460ced1b1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cxwpzbverwxdr929rb16f8m0q"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-HTTPFS-BASE"
        }
      }, {
        "name" : "hdfs-NAMENODE-386d77ab753d80c97f9872b4dda6d43c",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "9ffe1030-ce20-42f1-9b4d-33e80b1b1ce0"
        },
        "config" : {
          "items" : [ {
            "name" : "namenode_id",
            "value" : "74"
          }, {
            "name" : "role_jceks_password",
            "value" : "7cxcvwdsqt0jmejogel0bmvoi"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-NAMENODE-BASE"
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-52b05a4835689b61f2ad675eb1e77a3e",
        "type" : "SECONDARYNAMENODE",
        "hostRef" : {
          "hostId" : "49b066cc-69e7-4a85-ac3d-2173c6666aab"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bz3xc2hp1a4y7bg6url2yejeg"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-SECONDARYNAMENODE-BASE"
        }
      } ],
      "displayName" : "HDFS",
      "roleConfigGroups" : [ {
        "name" : "hdfs-BALANCER-BASE",
        "displayName" : "Balancer Default Group",
        "roleType" : "BALANCER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-1",
        "displayName" : "DataNode Group 1",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "2642411520"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-2",
        "displayName" : "DataNode Group 2",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "2227175424"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-3",
        "displayName" : "DataNode Group 3",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "1730150400"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-4",
        "displayName" : "DataNode Group 4",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "916455424"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "1191182336"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-BASE",
        "displayName" : "DataNode Default Group",
        "roleType" : "DATANODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "5367448780"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "2019557376"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-BASE",
        "displayName" : "Failover Controller Default Group",
        "roleType" : "FAILOVERCONTROLLER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-BASE",
        "displayName" : "HttpFS Default Group",
        "roleType" : "HTTPFS",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-BASE",
        "displayName" : "JournalNode Default Group",
        "roleType" : "JOURNALNODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-NAMENODE-BASE",
        "displayName" : "NameNode Default Group",
        "roleType" : "NAMENODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_handler_count",
            "value" : "32"
          }, {
            "name" : "dfs_namenode_service_handler_count",
            "value" : "32"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "1552941056"
          }, {
            "name" : "role_config_suppression_namenode_java_heapsize_minimum_validator",
            "value" : "true"
          } ]
        }
      }, {
        "name" : "hdfs-NFSGATEWAY-BASE",
        "displayName" : "NFS Gateway Default Group",
        "roleType" : "NFSGATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-BASE",
        "displayName" : "SecondaryNameNode Default Group",
        "roleType" : "SECONDARYNAMENODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "1552941056"
          } ]
        }
      } ],
      "replicationSchedules" : [ ],
      "snapshotPolicies" : [ ]
    } ],
    "parcels" : [ {
      "product" : "CDH",
      "version" : "5.8.5-1.cdh5.8.5.p0.5",
      "stage" : "DISTRIBUTED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    }, {
      "product" : "CDH",
      "version" : "5.8.5-1.cdh5.8.5.p0.5",
      "stage" : "ACTIVATED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "9ffe1030-ce20-42f1-9b4d-33e80b1b1ce0",
    "ipAddress" : "172.31.39.17",
    "hostname" : "ip-172-31-39-17.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "49b066cc-69e7-4a85-ac3d-2173c6666aab",
    "ipAddress" : "172.31.39.184",
    "hostname" : "ip-172-31-39-184.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "a1960418-6170-4067-834f-1d3460ced1b1",
    "ipAddress" : "172.31.44.186",
    "hostname" : "ip-172-31-44-186.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "d71ee147-1b3b-4eeb-b627-a75820f0262d",
    "ipAddress" : "172.31.45.113",
    "hostname" : "ip-172-31-45-113.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "905a41f4-92ce-4890-9f91-8da8a4ad75b5",
    "ipAddress" : "172.31.47.134",
    "hostname" : "ip-172-31-47-134.eu-central-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-3a872f1d47cf4d5711dcb5e260a0548a",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "fff8330099593dcf49a31d3d986b574ceb6dd3747ace7e1a2a1d394c79308ef8",
    "pwSalt" : -6225791900159240980,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-3a872f1d47cf4d5711dcb5e260a0548a",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "f14cd5ef1767eb14cf288dc1a2d71284e68b4ac5a3fbf32929f7abdfacc9af64",
    "pwSalt" : 4701674164475945066,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-3a872f1d47cf4d5711dcb5e260a0548a",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "89ddeaa6b1f587a10b28afe7a3947489a315111beaa4443c06150adb484896f9",
    "pwSalt" : -630756260612332290,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-3a872f1d47cf4d5711dcb5e260a0548a",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "25322fddfef2d00f9b5c4b1c9f4a5505e7aff0067d0afb60183426c2504286c1",
    "pwSalt" : -7547310827181884774,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "1b051335f2eae06959bb8f7abcf6447a7975a643948e0b20052003c3cb1d87d2",
    "pwSalt" : -1087996704053261996,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.11.2",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170811-0014",
    "gitHash" : "3c3ea33a12076fb83a8f11c4452c52fac685d01b",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-3a872f1d47cf4d5711dcb5e260a0548a",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "905a41f4-92ce-4890-9f91-8da8a4ad75b5"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "4jkctth5nufl3rujm1kawa6nn"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-ALERTPUBLISHER-BASE"
      }
    }, {
      "name" : "mgmt-EVENTSERVER-3a872f1d47cf4d5711dcb5e260a0548a",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "905a41f4-92ce-4890-9f91-8da8a4ad75b5"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "26kuss8x9bn8blr6xz7h6awtr"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-EVENTSERVER-BASE"
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-3a872f1d47cf4d5711dcb5e260a0548a",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "905a41f4-92ce-4890-9f91-8da8a4ad75b5"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "51609277v2nv47xn8pd0qmck8"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-HOSTMONITOR-BASE"
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-3a872f1d47cf4d5711dcb5e260a0548a",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "905a41f4-92ce-4890-9f91-8da8a4ad75b5"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "aqs5dfq8v8ajukboz52346ryv"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-REPORTSMANAGER-BASE"
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-3a872f1d47cf4d5711dcb5e260a0548a",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "905a41f4-92ce-4890-9f91-8da8a4ad75b5"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9ng8k17jf78vp86sft9bomdji"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-SERVICEMONITOR-BASE"
      }
    } ],
    "displayName" : "Cloudera Management Service",
    "roleConfigGroups" : [ {
      "name" : "mgmt-ACTIVITYMONITOR-BASE",
      "displayName" : "Activity Monitor Default Group",
      "roleType" : "ACTIVITYMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-ALERTPUBLISHER-BASE",
      "displayName" : "Alert Publisher Default Group",
      "roleType" : "ALERTPUBLISHER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-BASE",
      "displayName" : "Event Server Default Group",
      "roleType" : "EVENTSERVER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "916455424"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-BASE",
      "displayName" : "Host Monitor Default Group",
      "roleType" : "HOSTMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "916455424"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1191182336"
        } ]
      }
    }, {
      "name" : "mgmt-NAVIGATOR-BASE",
      "displayName" : "Navigator Audit Server Default Group",
      "roleType" : "NAVIGATOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-NAVIGATORMETASERVER-BASE",
      "displayName" : "Navigator Metadata Server Default Group",
      "roleType" : "NAVIGATORMETASERVER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-BASE",
      "displayName" : "Reports Manager Default Group",
      "roleType" : "REPORTSMANAGER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-44-186.eu-central-1.compute.internal"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_password"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "916455424"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-BASE",
      "displayName" : "Service Monitor Default Group",
      "roleType" : "SERVICEMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "916455424"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1191182336"
        } ]
      }
    }, {
      "name" : "mgmt-TELEMETRYPUBLISHER-BASE",
      "displayName" : "Telemetry Publisher Default Group",
      "roleType" : "TELEMETRYPUBLISHER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    } ]
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/25/2012 23:00"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh5/parcels/5.8/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,http://archive.cloudera.com/kudu/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  },
  "allHostsConfig" : {
    "items" : [ ]
  },
  "peers" : [ ],
  "hostTemplates" : {
    "items" : [ ]
  }
}
