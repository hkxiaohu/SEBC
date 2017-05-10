



### Use hdfs fsck <path> -files -blocks on source directory
```
[hdfs@ip-172-31-7-188 root]$ hdfs fsck /user/xiaohu-liu/source -files -blocks
Connecting to namenode via http://ip-172-31-0-239:50070
FSCK started by hdfs (auth:KERBEROS_SSL) from /172.31.7.188 for path /user/xiaohu-liu/source at Wed May 10 15:12:09 UTC 2017
/user/xiaohu-liu/source <dir>
/user/xiaohu-liu/source/_SUCCESS 0 bytes, 0 block(s):  OK

/user/xiaohu-liu/source/part-m-00000 524288000 bytes, 4 block(s):  OK
0. BP-1635622048-172.31.0.239-1494244538499:blk_1073743627_2803 len=134217728 Live_repl=3
1. BP-1635622048-172.31.0.239-1494244538499:blk_1073743628_2804 len=134217728 Live_repl=3
2. BP-1635622048-172.31.0.239-1494244538499:blk_1073743629_2805 len=134217728 Live_repl=3
3. BP-1635622048-172.31.0.239-1494244538499:blk_1073743630_2806 len=121634816 Live_repl=3

Status: HEALTHY
 Total size:	524288000 B
 Total dirs:	1
 Total files:	2
 Total symlinks:		0
 Total blocks (validated):	4 (avg. block size 131072000 B)
 Minimally replicated blocks:	4 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		4
 Number of racks:		1
FSCK ended at Wed May 10 15:12:09 UTC 2017 in 2 milliseconds


The filesystem under path '/user/xiaohu-liu/source' is HEALTHY
```

### Use hdfs fsck <path> -files -blocks on target directory
