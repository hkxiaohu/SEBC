### Choose a partner in class
```
luqimin2005
```

### Name a source directory after your GitHub handle && Name a target directory after your partner's GitHub handle
```
[root@ip-172-31-7-188 ~]# hadoop fs -ls /user  | grep -E "xiaohu-liu|luqimin2005"
drwxr-xr-x   - hdfs       supergroup          0 2017-05-09 04:40 /user/luqimin2005
drwxr-xr-x   - xiaohu-liu supergroup          0 2017-05-10 15:49 /user/xiaohu-liu

```

### Use teragen to create a 500 MB file
```
[hdfs@ip-172-31-7-188 root]$ hadoop fs -ls -h /user/xiaohu-liu/source
Found 2 items
-rw-r--r--   3 hdfs supergroup          0 2017-05-10 15:46 /user/xiaohu-liu/source/_SUCCESS
-rw-r--r--   3 hdfs supergroup      500 M 2017-05-10 15:46 /user/xiaohu-liu/source/part-m-00000

commands and output here:

[hdfs@ip-172-31-7-188 root]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -D mapreduce.job.maps=1  5242880 /user/xiaohu-liu/source
17/05/10 15:45:55 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-0-239/172.31.0.239:8032
17/05/10 15:45:56 INFO terasort.TeraSort: Generating 5242880 using 1
17/05/10 15:45:56 INFO mapreduce.JobSubmitter: number of splits:1
17/05/10 15:45:56 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494426924737_0003
17/05/10 15:45:56 INFO impl.YarnClientImpl: Submitted application application_1494426924737_0003
17/05/10 15:45:57 INFO mapreduce.Job: The url to track the job: http://ip-172-31-0-239:8088/proxy/application_1494426924737_0003/
17/05/10 15:45:57 INFO mapreduce.Job: Running job: job_1494426924737_0003
17/05/10 15:46:03 INFO mapreduce.Job: Job job_1494426924737_0003 running in uber mode : false
17/05/10 15:46:03 INFO mapreduce.Job:  map 0% reduce 0%
17/05/10 15:46:15 INFO mapreduce.Job:  map 73% reduce 0%
17/05/10 15:46:17 INFO mapreduce.Job:  map 100% reduce 0%
17/05/10 15:46:17 INFO mapreduce.Job: Job job_1494426924737_0003 completed successfully
17/05/10 15:46:17 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=123033
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=82
		HDFS: Number of bytes written=524288000
		HDFS: Number of read operations=4
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=2
	Job Counters 
		Launched map tasks=1
		Other local map tasks=1
		Total time spent by all maps in occupied slots (ms)=11702
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=11702
		Total vcore-seconds taken by all map tasks=11702
		Total megabyte-seconds taken by all map tasks=11982848
	Map-Reduce Framework
		Map input records=5242880
		Map output records=5242880
		Input split bytes=82
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=85
		CPU time spent (ms)=11580
		Physical memory (bytes) snapshot=366780416
		Virtual memory (bytes) snapshot=1565331456
		Total committed heap usage (bytes)=397934592
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=11257830824958050
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=524288000

```

### Use hdfs fsck <path> -files -blocks on source directory
```
[hdfs@ip-172-31-7-188 root]$ hdfs fsck /user/xiaohu-liu/source -files -blocks
Connecting to namenode via http://ip-172-31-0-239:50070
FSCK started by hdfs (auth:SIMPLE) from /172.31.7.188 for path /user/xiaohu-liu/source at Wed May 10 15:12:09 UTC 2017
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
```
[hdfs@ip-172-31-7-188 root]$ hdfs fsck /user/luqimin2005/target -files -blocks
Connecting to namenode via http://ip-172-31-2-22:50070
FSCK started by hdfs (auth:SIMPLE) from /172.31.2.22 for path /user/luqimin2005/target at Wed May 10 16:02:15 UTC 2017
/user/luqimin2005/target <dir>
/user/luqimin2005/target/_SUCCESS 0 bytes, 0 block(s):  OK

/user/luqimin2005/target/part-m-00000 524288000 bytes, 4 block(s):  OK
0. BP-1860349024-172.31.2.22-1494426862770:blk_1073742587_1763 len=134217728 Live_repl=3
1. BP-1860349024-172.31.2.22-1494426862770:blk_1073742588_1764 len=134217728 Live_repl=3
2. BP-1860349024-172.31.2.22-1494426862770:blk_1073742589_1765 len=134217728 Live_repl=3
3. BP-1860349024-172.31.2.22-1494426862770:blk_1073742590_1766 len=121634816 Live_repl=3

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
 Number of data-nodes:		3
 Number of racks:		1
FSCK ended at Wed May 10 16:02:15 UTC 2017 in 1 milliseconds


The filesystem under path '/user/luqimin2005/target' is HEALTHY

```
