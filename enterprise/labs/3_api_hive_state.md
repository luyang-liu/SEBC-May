* curl -X POST -u "admin:admin"  http://ec2-54-191-94-126.us-west-2.compute.amazonaws.com:7180/api/v14/clusters/luyang-liu/services/hive/commands/stop
```
 {
    "id" : 1075,
    "name" : "Stop",
    "startTime" : "2017-05-11T01:15:48.696Z",
    "active" : true,
    "serviceRef" : {
      "clusterName" : "cluster",
      "serviceName" : "hive"
    }
  }   
```
   
* curl -X POST -u "admin:admin"  http://ec2-54-191-94-126.us-west-2.compute.amazonaws.com:7180/api/v14/clusters/luyang-liu/services/hive/commands/start
``` 
{
    "id" : 1078,
    "name" : "Start",
    "startTime" : "2017-05-11T01:16:15.882Z",
    "active" : true,
    "serviceRef" : {
      "clusterName" : "cluster",
      "serviceName" : "hive"
    }
  } 
   
```

* curl -X GET -u "admin:admin"  http://ec2-54-191-94-126.us-west-2.compute.amazonaws.com:7180/api/v14/clusters/luyang-liu/services/hive
```
 {
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://ip-172-31-17-23.us-west-2.compute.internal:7180/cmf/serviceRedirect/hive",
  "roleInstancesUrl" : "http://ip-172-31-17-23.us-west-2.compute.internal:7180/cmf/serviceRedirect/hive/instances",
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
} 
```