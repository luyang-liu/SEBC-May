* Create a precious directory in HDFS; copy the ZIP course file into it.
`# hdfs dfs -mkdir /user/root/snapshort `
`# hdfs dfs -ls /user/root/`
Found 6 items
drwx------   - root supergroup          0 2017-05-09 21:02 /user/root/.Trash
drwx------   - root supergroup          0 2017-05-10 11:58 /user/root/.staging
drwxr-xr-x   - root supergroup          0 2017-05-10 11:58 /user/root/results
drwxr-xr-x   - root supergroup          0 2017-05-10 11:59 /user/root/snapshort
drwxr-xr-x   - root supergroup          0 2017-05-09 21:05 /user/root/teragen
drwxr-xr-x   - root supergroup          0 2017-05-09 10:23 /user/root/terasort 

`# hdfs dfs -copyFromLocal ./SEBC-Shanghai.zip /user/root/snapshort/ `
`# hdfs dfs -ls /user/root/snapshort`
Found 1 items
-rw-r--r--   3 root supergroup     474957 2017-05-10 12:11 /user/root/snapshort/SEBC-Shanghai.zip


* Enable snapshots for precious 
1:HDFS service>File Browser tab 
2:enabled snapshots for HDFS directory /user/root/snapshort :
Successfully enabled snapshots for HDFS directory /user/root/snapshort of service HDFS. 
Successfully created snapshot sebc-hdfs-test for HDFS directory /user/root/snapshort of service HDFS

* Create a snapshot called sebc-hdfs-test

* Delete the directory
# hdfs dfs -rm -r /user/root/snapshort
rm: Failed to move to trash: hdfs://ip-172-31-17-23.us-west-2.compute.internal:8020/user/root/snapshort: The directory /user/root/snapshort cannot be deleted since /user/root/snapshort is snapshottable and already has snapshots 

* Delete the ZIP file
# hdfs dfs -rm /user/root/snapshort/SEBC-Shanghai.zip
17/05/10 12:52:20 INFO fs.TrashPolicyDefault: Moved: 'hdfs://ip-172-31-17-23.us-west-2.compute.internal:8020/user/root/snapshort/SEBC-Shanghai.zip' to trash at: hdfs://ip-172-31-17-23.us-west-2.compute.internal:8020/user/root/.Trash/Current/user/root/snapshort/SEBC-Shanghai.zip

* Restore the deleted file
