0_replication.md:

### source directories

Connecting to namenode via http://ip-172-31-17-23.us-west-2.compute.internal:50070
FSCK started by root (auth:SIMPLE) from /172.31.21.165 for path /user/root/teragen/test-input500M at Tue May 09 20:56:12 EDT 2017
/user/root/teragen/test-input500M <dir>
/user/root/teragen/test-input500M/_SUCCESS 0 bytes, 0 block(s):  OK

/user/root/teragen/test-input500M/part-m-00000 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742905_2081 len=52428800 Live_repl=3

/user/root/teragen/test-input500M/part-m-00001 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742907_2083 len=52428800 Live_repl=3

/user/root/teragen/test-input500M/part-m-00002 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742909_2085 len=52428800 Live_repl=3

/user/root/teragen/test-input500M/part-m-00003 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742910_2086 len=52428800 Live_repl=3

/user/root/teragen/test-input500M/part-m-00004 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742904_2080 len=52428800 Live_repl=3

/user/root/teragen/test-input500M/part-m-00005 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742911_2087 len=52428800 Live_repl=3

/user/root/teragen/test-input500M/part-m-00006 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742908_2084 len=52428800 Live_repl=3

/user/root/teragen/test-input500M/part-m-00007 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742912_2088 len=52428800 Live_repl=3

/user/root/teragen/test-input500M/part-m-00008 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742906_2082 len=52428800 Live_repl=3

/user/root/teragen/test-input500M/part-m-00009 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742902_2078 len=52428800 Live_repl=3

Status: HEALTHY
 Total size:	524288000 B
 Total dirs:	1
 Total files:	11
 Total symlinks:		0
 Total blocks (validated):	10 (avg. block size 52428800 B)
 Minimally replicated blocks:	10 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		4
 Number of racks:		1
FSCK ended at Tue May 09 20:56:12 EDT 2017 in 4 milliseconds


The filesystem under path '/user/root/teragen/test-input500M' is HEALTHY


### target directories
Connecting to namenode via http://ip-172-31-17-23.us-west-2.compute.internal:50070
FSCK started by root (auth:SIMPLE) from /172.31.21.165 for path /user/root/teragen/test-output500M at Tue May 09 20:58:32 EDT 2017
/user/root/teragen/test-output500M <dir>
/user/root/teragen/test-output500M/_SUCCESS 0 bytes, 0 block(s):  OK

/user/root/teragen/test-output500M/part-m-00000 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742939_2115 len=52428800 Live_repl=3

/user/root/teragen/test-output500M/part-m-00001 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742940_2116 len=52428800 Live_repl=3

/user/root/teragen/test-output500M/part-m-00002 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742937_2113 len=52428800 Live_repl=3

/user/root/teragen/test-output500M/part-m-00003 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742944_2120 len=52428800 Live_repl=3

/user/root/teragen/test-output500M/part-m-00004 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742943_2119 len=52428800 Live_repl=3

/user/root/teragen/test-output500M/part-m-00005 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742941_2117 len=52428800 Live_repl=3

/user/root/teragen/test-output500M/part-m-00006 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742942_2118 len=52428800 Live_repl=3

/user/root/teragen/test-output500M/part-m-00007 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742936_2112 len=52428800 Live_repl=3

/user/root/teragen/test-output500M/part-m-00008 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742934_2110 len=52428800 Live_repl=3

/user/root/teragen/test-output500M/part-m-00009 52428800 bytes, 1 block(s):  OK
0. BP-693755600-172.31.17.23-1494324464742:blk_1073742935_2111 len=52428800 Live_repl=3

Status: HEALTHY
 Total size:	524288000 B
 Total dirs:	1
 Total files:	11
 Total symlinks:		0
 Total blocks (validated):	10 (avg. block size 52428800 B)
 Minimally replicated blocks:	10 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		4
 Number of racks:		1
FSCK ended at Tue May 09 20:58:32 EDT 2017 in 3 milliseconds


The filesystem under path '/user/root/teragen/test-output500M' is HEALTHY
