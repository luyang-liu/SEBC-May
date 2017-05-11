```
{
  "timestamp" : "2017-05-10T04:55:10.107Z",
  "clusters" : [ {
    "name" : "cluster",
    "displayName" : "luyang-liu",
    "version" : "CDH5",
    "fullVersion" : "5.9.2",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-17-23.us-west-2.compute.internal",
          "sensitive" : false
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "Hive_p",
          "sensitive" : true
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-429d5ff388d52ad92151863c5868cd2b",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-05efa5afe5fecb01f"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-593976cf47af06084a14cb288209f789",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0aae2043458bd36d4"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-6d97ed8791e4820be85e7b60dbc6854c",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0d29522d29e46cd28"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-88f1d4a3a231b1786159a55493c8fddb",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0df26de6d718458c6"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-fcc5832d6444fe3791b5342edc465aa1",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0803a12df9cd4e002"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-HIVEMETASTORE-429d5ff388d52ad92151863c5868cd2b",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "i-05efa5afe5fecb01f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7r8emfitk3edpewgh62qzlluo",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVEMETASTORE-BASE"
        }
      }, {
        "name" : "hive-HIVESERVER2-429d5ff388d52ad92151863c5868cd2b",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "i-05efa5afe5fecb01f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "c3lv46g42tumd7w8yzgnu7uxf",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVESERVER2-BASE"
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
            "value" : "576716800",
            "sensitive" : false
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
            "value" : "576716800",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "4160539852",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "700",
            "sensitive" : false
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
        "name" : "zookeeper-SERVER-429d5ff388d52ad92151863c5868cd2b",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-05efa5afe5fecb01f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "atjktli15furupe6g4c7sqcau",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "3",
            "sensitive" : false
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-593976cf47af06084a14cb288209f789",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-0aae2043458bd36d4"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ao0i4nrvnmyxip7lwnapkmmp3",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "1",
            "sensitive" : false
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-fcc5832d6444fe3791b5342edc465aa1",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-0803a12df9cd4e002"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2yq0emqj48mo8gkpw0e46cjwh",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "2",
            "sensitive" : false
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
          "items" : [ {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "576716800",
            "sensitive" : false
          } ]
        }
      } ]
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-17-23.us-west-2.compute.internal",
          "sensitive" : false
        }, {
          "name" : "database_password",
          "value" : "Hue_p",
          "sensitive" : true
        }, {
          "name" : "database_type",
          "value" : "mysql",
          "sensitive" : false
        }, {
          "name" : "hive_service",
          "value" : "hive",
          "sensitive" : false
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-429d5ff388d52ad92151863c5868cd2b",
          "sensitive" : false
        }, {
          "name" : "oozie_service",
          "value" : "oozie",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-429d5ff388d52ad92151863c5868cd2b",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "i-05efa5afe5fecb01f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6xmcxhgmlju0trs0d5wzzf32p",
            "sensitive" : true
          }, {
            "name" : "secret_key",
            "value" : "bi7nvwXzGUwZLBIyE5a6Xdt8o0ekKb",
            "sensitive" : true
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
          "value" : "hive",
          "sensitive" : false
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-429d5ff388d52ad92151863c5868cd2b",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "i-05efa5afe5fecb01f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2m9se4odcozw28euaoi5s92og",
            "sensitive" : true
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
            "value" : "ip-172-31-17-23.us-west-2.compute.internal",
            "sensitive" : false
          }, {
            "name" : "oozie_database_password",
            "value" : "Oozie_p",
            "sensitive" : true
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql",
            "sensitive" : false
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie",
            "sensitive" : false
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "576716800",
            "sensitive" : false
          } ]
        }
      } ]
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs",
          "sensitive" : false
        }, {
          "name" : "rm_dirty",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "VPDRzsH24WKfKpc0JGo326wB4cO8V4",
          "sensitive" : true
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-429d5ff388d52ad92151863c5868cd2b",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "i-05efa5afe5fecb01f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "x1mvx1qulreqhxe240r8q3si",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-JOBHISTORY-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-593976cf47af06084a14cb288209f789",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0aae2043458bd36d4"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "elgi39blu8ndmb23zidhbdxl3",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-1"
        }
      }, {
        "name" : "yarn-NODEMANAGER-6d97ed8791e4820be85e7b60dbc6854c",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0d29522d29e46cd28"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "a33b7sdqzg9fbyc458mtgi6l0",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-88f1d4a3a231b1786159a55493c8fddb",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0df26de6d718458c6"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "d707th6bqf1wivx6awclruquk",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-fcc5832d6444fe3791b5342edc465aa1",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0803a12df9cd4e002"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ehdd2ms7xvmbput3bh5r1ulpy",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-1"
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-429d5ff388d52ad92151863c5868cd2b",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "i-05efa5afe5fecb01f"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "57",
            "sensitive" : false
          }, {
            "name" : "role_jceks_password",
            "value" : "2dv5qe1gov48lohbrgzdh3kbj",
            "sensitive" : true
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
            "value" : "8",
            "sensitive" : false
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2",
            "sensitive" : false
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
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "576716800",
            "sensitive" : false
          } ]
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
            "value" : "100",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "4668",
            "sensitive" : false
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
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "5999",
            "sensitive" : false
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
            "name" : "resource_manager_java_heapsize",
            "value" : "576716800",
            "sensitive" : false
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "5999",
            "sensitive" : false
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "4",
            "sensitive" : false
          } ]
        }
      } ]
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "vD18IF8sYmWsNwTjoRCG6AEZp2he0K",
          "sensitive" : true
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "7QWvK2iuXnwYT8BuPHVAraGzKYGpVc",
          "sensitive" : true
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "8uKf9w8LZWgkwJMoQ4lrVcdBwNdGhN",
          "sensitive" : true
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-429d5ff388d52ad92151863c5868cd2b",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "i-05efa5afe5fecb01f"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-BALANCER-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-593976cf47af06084a14cb288209f789",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0aae2043458bd36d4"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "emrf1t6oj42bmit7ateltdsys",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-6d97ed8791e4820be85e7b60dbc6854c",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0d29522d29e46cd28"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "22xwjza7x3ha9w8hk9gv0hvgs",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-88f1d4a3a231b1786159a55493c8fddb",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0df26de6d718458c6"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ae0o58lumgx0xqsh9vidhxxkf",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-fcc5832d6444fe3791b5342edc465aa1",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0803a12df9cd4e002"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "nkp9vwcesjs64i6uq2ukcwr1",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-NAMENODE-429d5ff388d52ad92151863c5868cd2b",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-05efa5afe5fecb01f"
        },
        "config" : {
          "items" : [ {
            "name" : "namenode_id",
            "value" : "59",
            "sensitive" : false
          }, {
            "name" : "role_jceks_password",
            "value" : "cj7yr3zl677wbw04w0854l0yz",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-NAMENODE-BASE"
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-429d5ff388d52ad92151863c5868cd2b",
        "type" : "SECONDARYNAMENODE",
        "hostRef" : {
          "hostId" : "i-05efa5afe5fecb01f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3a66zha7fzz1c1gfyyo9xl3iu",
            "sensitive" : true
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
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "576716800",
            "sensitive" : false
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
            "value" : "/dfs/dn",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "3170565324",
            "sensitive" : false
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
            "value" : "true",
            "sensitive" : false
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
            "value" : "/dfs/nn",
            "sensitive" : false
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022",
            "sensitive" : false
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
            "value" : "/dfs/snn",
            "sensitive" : false
          } ]
        }
      } ],
      "replicationSchedules" : [ ],
      "snapshotPolicies" : [ ]
    } ],
    "parcels" : [ {
      "product" : "CDH",
      "version" : "5.9.2-1.cdh5.9.2.p0.3",
      "stage" : "DISTRIBUTED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    }, {
      "product" : "CDH",
      "version" : "5.9.2-1.cdh5.9.2.p0.3",
      "stage" : "ACTIVATED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "i-05efa5afe5fecb01f",
    "ipAddress" : "172.31.17.23",
    "hostname" : "ip-172-31-17-23.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ {
        "name" : "host_config_suppression_memory_overcommitted_validator",
        "value" : "true",
        "sensitive" : false
      } ]
    }
  }, {
    "hostId" : "i-0aae2043458bd36d4",
    "ipAddress" : "172.31.19.158",
    "hostname" : "ip-172-31-19-158.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0803a12df9cd4e002",
    "ipAddress" : "172.31.19.19",
    "hostname" : "ip-172-31-19-19.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0d29522d29e46cd28",
    "ipAddress" : "172.31.21.165",
    "hostname" : "ip-172-31-21-165.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0df26de6d718458c6",
    "ipAddress" : "172.31.25.63",
    "hostname" : "ip-172-31-25-63.us-west-2.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-429d5ff388d52ad92151863c5868cd2b",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "a3db7b256cd24061f70b37d9fe22ef3e8d6110825c9293c741670b369899118c",
    "pwSalt" : -2027510652988784285,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-429d5ff388d52ad92151863c5868cd2b",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "1fd701ba5bea31cc5d1f2c1c3c43662f60050c6f88179bf69cdbad7e90b1bee4",
    "pwSalt" : 475188740212044505,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-NAVIGATOR-429d5ff388d52ad92151863c5868cd2b",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "1f9d5c03ecf395906999c05c89cb3eee738da74cf4705478e44b25ad81f11852",
    "pwSalt" : 1502606863310090345,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-NAVIGATORMETASERVER-429d5ff388d52ad92151863c5868cd2b",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "526c9a91adb865338aef50415f026d60d8c833038b8c0a655f5f4c4f4b4f51f4",
    "pwSalt" : 7641096300513104726,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-429d5ff388d52ad92151863c5868cd2b",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "50784b3bc6578d5bdace0e9e673cf85394873a4d3b915b0c2d10b889d117a440",
    "pwSalt" : -7922438329218058593,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-429d5ff388d52ad92151863c5868cd2b",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "527ae708e696d7b330106ffe89c9f71f68d4ac744e2b1a4e3ce9f638a6196f49",
    "pwSalt" : 3240100875622751302,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "579dd86baaac2af7fed5732b688472a375b7cbb5840df89e6bfcab7cbd40e0f6",
    "pwSalt" : -1734287232619418717,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "5c8bbe14bea0e80d775c8b77a7a6dcc481b4831e2a581bedf6c1db6805aa31dd",
    "pwSalt" : 1323461821688799488,
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
      "items" : [ {
        "name" : "service_health_suppression_mgmt_navigatormetaserver_health",
        "value" : "true",
        "sensitive" : false
      } ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-429d5ff388d52ad92151863c5868cd2b",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "i-05efa5afe5fecb01f"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "28z410wufhchv6pgpnn1997ui",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-ALERTPUBLISHER-BASE"
      }
    }, {
      "name" : "mgmt-EVENTSERVER-429d5ff388d52ad92151863c5868cd2b",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "i-05efa5afe5fecb01f"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "cxfti2hjk2xmyedjin7j8qzv0",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-EVENTSERVER-BASE"
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-429d5ff388d52ad92151863c5868cd2b",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "i-05efa5afe5fecb01f"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "cekzzn6rnxj55n9kggzm5ddnu",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-HOSTMONITOR-BASE"
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-429d5ff388d52ad92151863c5868cd2b",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "i-05efa5afe5fecb01f"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "3prgg9sisl8ildrfweny8zsat",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-REPORTSMANAGER-BASE"
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-429d5ff388d52ad92151863c5868cd2b",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "i-05efa5afe5fecb01f"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "3x8ngw6oh9tgzbudom4b7nmdn",
          "sensitive" : true
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
          "value" : "576716800",
          "sensitive" : false
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
          "value" : "576716800",
          "sensitive" : false
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368",
          "sensitive" : false
        }, {
          "name" : "role_config_suppression_firehose_heap_size_validator",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "role_config_suppression_firehose_non_java_memory_validator",
          "value" : "true",
          "sensitive" : false
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
        "items" : [ {
          "name" : "navigator_database_host",
          "value" : "ip-172-31-17-23.us-west-2.compute.internal",
          "sensitive" : false
        }, {
          "name" : "navigator_database_password",
          "value" : "nav",
          "sensitive" : true
        }, {
          "name" : "navigator_heapsize",
          "value" : "576716800",
          "sensitive" : false
        } ]
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
        "items" : [ {
          "name" : "nav_metaserver_database_host",
          "value" : "ip-172-31-17-23.us-west-2.compute.internal",
          "sensitive" : false
        }, {
          "name" : "nav_metaserver_database_password",
          "value" : "navms",
          "sensitive" : true
        }, {
          "name" : "navigator_heapsize",
          "value" : "576716800",
          "sensitive" : false
        } ]
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
          "value" : "ip-172-31-17-23.us-west-2.compute.internal",
          "sensitive" : false
        }, {
          "name" : "headlamp_database_name",
          "value" : "amon",
          "sensitive" : false
        }, {
          "name" : "headlamp_database_password",
          "value" : "Amon_p",
          "sensitive" : true
        }, {
          "name" : "headlamp_database_user",
          "value" : "amon",
          "sensitive" : false
        }, {
          "name" : "headlamp_heapsize",
          "value" : "576716800",
          "sensitive" : false
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
          "value" : "576716800",
          "sensitive" : false
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368",
          "sensitive" : false
        }, {
          "name" : "role_config_suppression_firehose_heap_size_validator",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "role_config_suppression_firehose_non_java_memory_validator",
          "value" : "true",
          "sensitive" : false
        } ]
      }
    } ]
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/21/2012 17:50",
      "sensitive" : false
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD",
      "sensitive" : false
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/",
      "sensitive" : false
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
```