* What is ubertask optimization?
runs "sufficiently small" jobs sequentially within a single JVM. "Small" is defined by the mapreduce.job.ubertask.maxmaps, mapreduce.job.ubertask.maxreduces, and mapreduce.job.ubertask.maxbytes settings

* Where in CM is the Kerberos Security Realm value displayed?


* Which CDH service(s) host a property for enabling Kerberos authentication?
 
 
* How do you upgrade the CM agents?


* Give the tsquery statement used to chart Hue's CPU utilization?
SELECT cpu_system_rate + cpu_user_rate WHERE entityName = "hue-HUE_SERVER-429d5ff388d52ad92151863c5868cd2b" AND category = ROLE 


* Name all the roles that make up the Hive service
Hive Metastore Server  Gateway  HiveServer2  
* What steps must be completed before integrating Cloudera Manager with Kerberos?
Configure TLS encryption between Cloudera Manager Server and all cluster hosts
