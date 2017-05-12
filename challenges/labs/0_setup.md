### Challenge Setup
```
* cloud provider:AWS
* IP address and NDS name:
   Public :
   IP:54-186-198-129 DNS (IPv4)ec2-54-186-198-129.us-west-2.compute.amazonaws.com
   IP:54.202.229.53 DNS (IPv4)ec2-54-202-229-53.us-west-2.compute.amazonaws.com  
   IP:54.213.23.191 DNS (IPv4)ec2-54-213-23-191.us-west-2.compute.amazonaws.com
   IP:54-202-31-28 DNS (IPv4)ec2-54-202-31-28.us-west-2.compute.amazonaws.com
   IP:54-200-205-5 DNS (IPv4)ec2-54-200-205-5.us-west-2.compute.amazonaws.com

* Linux release 
   /* cat /proc/version  */
  Linux version 2.6.32-504.16.2.el6.x86_64 (mockbuild@x86-028.build.eng.bos.redhat.com) (gcc version 4.4.7 20120313 (Red Hat 4.4.7-9) (GCC) ) #1 SMP Tue Mar 10 17:01:00 EDT 2015
  

 * disk capacity available of my fist node
   /* df -h*/
  $df -h
    Filesystem      Size  Used Avail Use% Mounted on
    /dev/xvda1       30G  3.5G   25G  13% /
    tmpfs           7.8G     0  7.8G   0% /dev/shm
                                                   
  * yum repolist
   $yum repolist enabled
    Loaded plugins: amazon-id, rhui-lb, search-disabled-repos, security
    rhui-REGION-client-config-server-6                                                                                                                                      | 2.9 kB     00:00     
    rhui-REGION-rhel-server-releases                                                                                                                                        | 3.5 kB     00:00     
    rhui-REGION-rhel-server-rh-common                                                                                                                                       | 3.8 kB     00:00     
    repo id                                                                       repo name                                                                                                  status
    mysql-connectors-community                                                    MySQL Connectors Community                                                                                     36
    mysql-tools-community                                                         MySQL Tools Community                                                                                          47
    mysql56-community                                                             MySQL 5.6 Community Server                                                                                    358
    rhui-REGION-client-config-server-6                                            Red Hat Update Infrastructure 2.0 Client Configuration Server 6                                                 7
    rhui-REGION-rhel-server-releases                                              Red Hat Enterprise Linux Server 6 (RPMs)                                                                   19,498
    rhui-REGION-rhel-server-rh-common                                             Red Hat Enterprise Linux Server 6 RH Common (RPMs)                                                            129
    repolist: 20,075

```

