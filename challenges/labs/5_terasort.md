### Copy the command and full output to challenges/labs/5_terasort.md
```
[zhou@ip-172-31-7-7 yum.repos.d]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/zhou/tgen /user/zhou/tsort
17/05/12 02:52:35 INFO terasort.TeraSort: starting
17/05/12 02:52:36 INFO hdfs.DFSClient: Created token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@XIAOHU-LIU.CN, renewer=yarn, realUser=, issueDate=1494557556778, maxDate=1495162356778, sequenceNumber=1, masterKeyId=2 on 172.31.4.25:8020
17/05/12 02:52:36 INFO security.TokenCache: Got dt for hdfs://ip-172-31-4-25:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.4.25:8020, Ident: (token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@XIAOHU-LIU.CN, renewer=yarn, realUser=, issueDate=1494557556778, maxDate=1495162356778, sequenceNumber=1, masterKeyId=2)
17/05/12 02:52:36 INFO input.FileInputFormat: Total input paths to process : 6
Spent 344ms computing base-splits.
Spent 3ms computing TeraScheduler splits.
Computing input splits took 348ms
Sampling 10 splits of 102
Making 20 from 100000 sampled records
Computing parititions took 584ms
Spent 935ms computing partitions.
17/05/12 02:52:37 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-3-172/172.31.3.172:8032
17/05/12 02:52:38 INFO mapreduce.JobSubmitter: number of splits:102
17/05/12 02:52:38 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494557335908_0001
17/05/12 02:52:38 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.4.25:8020, Ident: (token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@XIAOHU-LIU.CN, renewer=yarn, realUser=, issueDate=1494557556778, maxDate=1495162356778, sequenceNumber=1, masterKeyId=2)
17/05/12 02:52:39 INFO impl.YarnClientImpl: Submitted application application_1494557335908_0001
17/05/12 02:52:39 INFO mapreduce.Job: The url to track the job: http://ip-172-31-3-172:8088/proxy/application_1494557335908_0001/
17/05/12 02:52:39 INFO mapreduce.Job: Running job: job_1494557335908_0001
17/05/12 02:52:48 INFO mapreduce.Job: Job job_1494557335908_0001 running in uber mode : false
17/05/12 02:52:48 INFO mapreduce.Job:  map 0% reduce 0%
17/05/12 02:52:58 INFO mapreduce.Job:  map 1% reduce 0%
17/05/12 02:52:59 INFO mapreduce.Job:  map 4% reduce 0%
17/05/12 02:53:05 INFO mapreduce.Job:  map 7% reduce 0%
17/05/12 02:53:06 INFO mapreduce.Job:  map 8% reduce 0%
17/05/12 02:53:11 INFO mapreduce.Job:  map 10% reduce 0%
17/05/12 02:53:12 INFO mapreduce.Job:  map 11% reduce 0%
17/05/12 02:53:13 INFO mapreduce.Job:  map 12% reduce 0%
17/05/12 02:53:18 INFO mapreduce.Job:  map 15% reduce 0%
17/05/12 02:53:21 INFO mapreduce.Job:  map 16% reduce 0%
17/05/12 02:53:25 INFO mapreduce.Job:  map 19% reduce 0%
17/05/12 02:53:28 INFO mapreduce.Job:  map 20% reduce 0%
17/05/12 02:53:31 INFO mapreduce.Job:  map 21% reduce 0%
17/05/12 02:53:32 INFO mapreduce.Job:  map 23% reduce 0%
17/05/12 02:53:34 INFO mapreduce.Job:  map 24% reduce 0%
17/05/12 02:53:37 INFO mapreduce.Job:  map 25% reduce 0%
17/05/12 02:53:39 INFO mapreduce.Job:  map 26% reduce 0%
17/05/12 02:53:41 INFO mapreduce.Job:  map 27% reduce 0%
17/05/12 02:53:44 INFO mapreduce.Job:  map 28% reduce 0%
17/05/12 02:53:46 INFO mapreduce.Job:  map 30% reduce 0%
17/05/12 02:53:48 INFO mapreduce.Job:  map 31% reduce 0%
17/05/12 02:53:51 INFO mapreduce.Job:  map 32% reduce 0%
17/05/12 02:53:53 INFO mapreduce.Job:  map 34% reduce 0%
17/05/12 02:53:55 INFO mapreduce.Job:  map 35% reduce 0%
17/05/12 02:53:57 INFO mapreduce.Job:  map 36% reduce 0%
17/05/12 02:53:59 INFO mapreduce.Job:  map 37% reduce 0%
17/05/12 02:54:00 INFO mapreduce.Job:  map 38% reduce 0%
17/05/12 02:54:02 INFO mapreduce.Job:  map 39% reduce 0%
17/05/12 02:54:03 INFO mapreduce.Job:  map 40% reduce 0%
17/05/12 02:54:06 INFO mapreduce.Job:  map 41% reduce 0%
17/05/12 02:54:07 INFO mapreduce.Job:  map 42% reduce 0%
17/05/12 02:54:09 INFO mapreduce.Job:  map 43% reduce 0%
17/05/12 02:54:10 INFO mapreduce.Job:  map 44% reduce 0%
17/05/12 02:54:13 INFO mapreduce.Job:  map 46% reduce 0%
17/05/12 02:54:16 INFO mapreduce.Job:  map 47% reduce 0%
17/05/12 02:54:17 INFO mapreduce.Job:  map 48% reduce 0%
17/05/12 02:54:19 INFO mapreduce.Job:  map 49% reduce 0%
17/05/12 02:54:20 INFO mapreduce.Job:  map 50% reduce 0%
17/05/12 02:54:23 INFO mapreduce.Job:  map 52% reduce 0%
17/05/12 02:54:25 INFO mapreduce.Job:  map 53% reduce 0%
17/05/12 02:54:27 INFO mapreduce.Job:  map 54% reduce 0%
17/05/12 02:54:30 INFO mapreduce.Job:  map 56% reduce 0%
17/05/12 02:54:32 INFO mapreduce.Job:  map 57% reduce 0%
17/05/12 02:54:34 INFO mapreduce.Job:  map 58% reduce 0%
17/05/12 02:54:37 INFO mapreduce.Job:  map 60% reduce 0%
17/05/12 02:54:39 INFO mapreduce.Job:  map 61% reduce 0%
17/05/12 02:54:41 INFO mapreduce.Job:  map 62% reduce 0%
17/05/12 02:54:44 INFO mapreduce.Job:  map 64% reduce 0%
17/05/12 02:54:45 INFO mapreduce.Job:  map 65% reduce 0%
17/05/12 02:54:48 INFO mapreduce.Job:  map 66% reduce 0%
17/05/12 02:54:51 INFO mapreduce.Job:  map 68% reduce 0%
17/05/12 02:54:52 INFO mapreduce.Job:  map 69% reduce 0%
17/05/12 02:54:55 INFO mapreduce.Job:  map 70% reduce 0%
17/05/12 02:54:57 INFO mapreduce.Job:  map 71% reduce 0%
17/05/12 02:54:58 INFO mapreduce.Job:  map 72% reduce 0%
17/05/12 02:54:59 INFO mapreduce.Job:  map 73% reduce 0%
17/05/12 02:55:02 INFO mapreduce.Job:  map 74% reduce 0%
17/05/12 02:55:04 INFO mapreduce.Job:  map 75% reduce 0%
17/05/12 02:55:05 INFO mapreduce.Job:  map 76% reduce 0%
17/05/12 02:55:08 INFO mapreduce.Job:  map 77% reduce 0%
17/05/12 02:55:11 INFO mapreduce.Job:  map 78% reduce 0%
17/05/12 02:55:12 INFO mapreduce.Job:  map 80% reduce 0%
17/05/12 02:55:15 INFO mapreduce.Job:  map 81% reduce 0%
17/05/12 02:55:18 INFO mapreduce.Job:  map 82% reduce 0%
17/05/12 02:55:19 INFO mapreduce.Job:  map 84% reduce 0%
17/05/12 02:55:23 INFO mapreduce.Job:  map 85% reduce 0%
17/05/12 02:55:25 INFO mapreduce.Job:  map 86% reduce 0%
17/05/12 02:55:29 INFO mapreduce.Job:  map 86% reduce 1%
17/05/12 02:55:30 INFO mapreduce.Job:  map 87% reduce 3%
17/05/12 02:55:32 INFO mapreduce.Job:  map 88% reduce 3%
17/05/12 02:55:37 INFO mapreduce.Job:  map 89% reduce 3%
17/05/12 02:55:38 INFO mapreduce.Job:  map 90% reduce 3%
17/05/12 02:55:42 INFO mapreduce.Job:  map 91% reduce 3%
17/05/12 02:55:44 INFO mapreduce.Job:  map 92% reduce 3%
17/05/12 02:55:47 INFO mapreduce.Job:  map 93% reduce 3%
17/05/12 02:55:51 INFO mapreduce.Job:  map 94% reduce 3%
17/05/12 02:55:53 INFO mapreduce.Job:  map 95% reduce 3%
17/05/12 02:55:56 INFO mapreduce.Job:  map 96% reduce 3%
17/05/12 02:55:59 INFO mapreduce.Job:  map 97% reduce 3%
17/05/12 02:56:02 INFO mapreduce.Job:  map 98% reduce 3%
17/05/12 02:56:05 INFO mapreduce.Job:  map 99% reduce 3%
17/05/12 02:56:07 INFO mapreduce.Job:  map 100% reduce 3%
17/05/12 02:56:08 INFO mapreduce.Job:  map 100% reduce 4%
17/05/12 02:56:10 INFO mapreduce.Job:  map 100% reduce 5%
17/05/12 02:56:11 INFO mapreduce.Job:  map 100% reduce 6%
17/05/12 02:56:13 INFO mapreduce.Job:  map 100% reduce 8%
17/05/12 02:56:14 INFO mapreduce.Job:  map 100% reduce 14%
17/05/12 02:56:16 INFO mapreduce.Job:  map 100% reduce 19%
17/05/12 02:56:18 INFO mapreduce.Job:  map 100% reduce 20%
17/05/12 02:56:23 INFO mapreduce.Job:  map 100% reduce 24%
17/05/12 02:56:24 INFO mapreduce.Job:  map 100% reduce 28%
17/05/12 02:56:25 INFO mapreduce.Job:  map 100% reduce 29%
17/05/12 02:56:26 INFO mapreduce.Job:  map 100% reduce 34%
17/05/12 02:56:27 INFO mapreduce.Job:  map 100% reduce 39%
17/05/12 02:56:28 INFO mapreduce.Job:  map 100% reduce 40%
17/05/12 02:56:34 INFO mapreduce.Job:  map 100% reduce 44%
17/05/12 02:56:35 INFO mapreduce.Job:  map 100% reduce 45%
17/05/12 02:56:36 INFO mapreduce.Job:  map 100% reduce 49%
17/05/12 02:56:37 INFO mapreduce.Job:  map 100% reduce 53%
17/05/12 02:56:38 INFO mapreduce.Job:  map 100% reduce 58%
17/05/12 02:56:39 INFO mapreduce.Job:  map 100% reduce 60%
17/05/12 02:56:45 INFO mapreduce.Job:  map 100% reduce 64%
17/05/12 02:56:47 INFO mapreduce.Job:  map 100% reduce 65%
17/05/12 02:56:48 INFO mapreduce.Job:  map 100% reduce 69%
17/05/12 02:56:49 INFO mapreduce.Job:  map 100% reduce 77%
17/05/12 02:56:50 INFO mapreduce.Job:  map 100% reduce 79%
17/05/12 02:56:52 INFO mapreduce.Job:  map 100% reduce 80%
17/05/12 02:56:57 INFO mapreduce.Job:  map 100% reduce 84%
17/05/12 02:56:59 INFO mapreduce.Job:  map 100% reduce 89%
17/05/12 02:57:00 INFO mapreduce.Job:  map 100% reduce 93%
17/05/12 02:57:01 INFO mapreduce.Job:  map 100% reduce 98%
17/05/12 02:57:02 INFO mapreduce.Job:  map 100% reduce 99%
17/05/12 02:57:03 INFO mapreduce.Job:  map 100% reduce 100%
17/05/12 02:57:03 INFO mapreduce.Job: Job job_1494557335908_0001 completed successfully
17/05/12 02:57:03 INFO mapreduce.Job: Counters: 50
	File System Counters
		FILE: Number of bytes read=2924253417
		FILE: Number of bytes written=5812602506
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=6553612138
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=366
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=40
	Job Counters 
		Launched map tasks=102
		Launched reduce tasks=20
		Data-local map tasks=98
		Rack-local map tasks=4
		Total time spent by all maps in occupied slots (ms)=574676
		Total time spent by all reduces in occupied slots (ms)=291895
		Total time spent by all map tasks (ms)=574676
		Total time spent by all reduce tasks (ms)=291895
		Total vcore-seconds taken by all map tasks=574676
		Total vcore-seconds taken by all reduce tasks=291895
		Total megabyte-seconds taken by all map tasks=588468224
		Total megabyte-seconds taken by all reduce tasks=298900480
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Map output bytes=6684672000
		Map output materialized bytes=2873129181
		Input split bytes=12138
		Combine input records=0
		Combine output records=0
		Reduce input groups=65536000
		Reduce shuffle bytes=2873129181
		Reduce input records=65536000
		Reduce output records=65536000
		Spilled Records=131072000
		Shuffled Maps =2040
		Failed Shuffles=0
		Merged Map outputs=2040
		GC time elapsed (ms)=9804
		CPU time spent (ms)=612030
		Physical memory (bytes) snapshot=65956376576
		Virtual memory (bytes) snapshot=193266184192
		Total committed heap usage (bytes)=73078931456
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=6553600000
	File Output Format Counters 
		Bytes Written=6553600000
17/05/12 02:57:03 INFO terasort.TeraSort: done

real	4m29.160s
user	0m7.149s
sys	0m0.788s
```
