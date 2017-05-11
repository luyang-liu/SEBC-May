
### Use the api to check:
```
* $curl -X GET -u "admin:admin"  http://ec2-54-191-94-126.us-west-2.compute.amazonaws.com:7180/api/version
   `v16`
* $curl -X GET -u "admin:admin"  http://ec2-54-191-94-126.us-west-2.compute.amazonaws.com:7180/api/v16/cm/version
{
  "version" : "5.11.0",
  "buildUser" : "jenkins",
  "buildTimestamp" : "20170412-1249",
  "gitHash" : "70cb1442626406432a6e7af5bdf206a384ca3f98",
  "snapshot" : false
}
* $curl -X GET -u "admin:admin"  http://ec2-54-191-94-126.us-west-2.compute.amazonaws.com:7180/api/v16/users
{
  "items" : [ {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ]
  }, {
    "name" : "luyang-liu",
    "roles" : [ "ROLE_ADMIN" ]
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ]
  } ]
}


* curl -X GET -u "admin:admin"  http://ec2-54-191-94-126.us-west-2.compute.amazonaws.com:7180/api/v16/cm/scmDbInfo
{
  "scmDbType" : "MYSQL",
  "embeddedDbUsed" : false
}

```