
```
[xiaohu-liu@ip-172-31-7-188 root]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -D mapreduce.job.maps=4 -D dfs.blocksize=32M  104857600 /user/xiaohu-liu/terasort-input
17/05/09 05:44:26 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-0-239/172.31.0.239:8032
17/05/09 05:44:26 INFO terasort.TeraSort: Generating 104857600 using 4
17/05/09 05:44:27 INFO mapreduce.JobSubmitter: number of splits:4
17/05/09 05:44:27 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494292583990_0006
17/05/09 05:44:27 INFO impl.YarnClientImpl: Submitted application application_1494292583990_0006
17/05/09 05:44:27 INFO mapreduce.Job: The url to track the job: http://ip-172-31-0-239:8088/proxy/application_1494292583990_0006/
17/05/09 05:44:27 INFO mapreduce.Job: Running job: job_1494292583990_0006
17/05/09 05:44:35 INFO mapreduce.Job: Job job_1494292583990_0006 running in uber mode : false
17/05/09 05:44:35 INFO mapreduce.Job:  map 0% reduce 0%
17/05/09 05:44:47 INFO mapreduce.Job:  map 7% reduce 0%
17/05/09 05:44:48 INFO mapreduce.Job:  map 9% reduce 0%
17/05/09 05:44:50 INFO mapreduce.Job:  map 13% reduce 0%
17/05/09 05:44:51 INFO mapreduce.Job:  map 14% reduce 0%
17/05/09 05:44:53 INFO mapreduce.Job:  map 17% reduce 0%
17/05/09 05:44:54 INFO mapreduce.Job:  map 18% reduce 0%
17/05/09 05:44:56 INFO mapreduce.Job:  map 20% reduce 0%
17/05/09 05:44:59 INFO mapreduce.Job:  map 23% reduce 0%
17/05/09 05:45:02 INFO mapreduce.Job:  map 25% reduce 0%
17/05/09 05:45:05 INFO mapreduce.Job:  map 27% reduce 0%
17/05/09 05:45:08 INFO mapreduce.Job:  map 29% reduce 0%
17/05/09 05:45:11 INFO mapreduce.Job:  map 31% reduce 0%
17/05/09 05:45:14 INFO mapreduce.Job:  map 34% reduce 0%
17/05/09 05:45:17 INFO mapreduce.Job:  map 36% reduce 0%
17/05/09 05:45:20 INFO mapreduce.Job:  map 39% reduce 0%
17/05/09 05:45:23 INFO mapreduce.Job:  map 41% reduce 0%
17/05/09 05:45:26 INFO mapreduce.Job:  map 43% reduce 0%
17/05/09 05:45:29 INFO mapreduce.Job:  map 45% reduce 0%
17/05/09 05:45:32 INFO mapreduce.Job:  map 48% reduce 0%
17/05/09 05:45:35 INFO mapreduce.Job:  map 50% reduce 0%
17/05/09 05:45:38 INFO mapreduce.Job:  map 53% reduce 0%
17/05/09 05:45:41 INFO mapreduce.Job:  map 55% reduce 0%
17/05/09 05:45:44 INFO mapreduce.Job:  map 57% reduce 0%
17/05/09 05:45:47 INFO mapreduce.Job:  map 59% reduce 0%
17/05/09 05:45:50 INFO mapreduce.Job:  map 62% reduce 0%
17/05/09 05:45:53 INFO mapreduce.Job:  map 64% reduce 0%
17/05/09 05:45:56 INFO mapreduce.Job:  map 66% reduce 0%
17/05/09 05:46:00 INFO mapreduce.Job:  map 68% reduce 0%
17/05/09 05:46:03 INFO mapreduce.Job:  map 70% reduce 0%
17/05/09 05:46:06 INFO mapreduce.Job:  map 73% reduce 0%
17/05/09 05:46:09 INFO mapreduce.Job:  map 75% reduce 0%
17/05/09 05:46:12 INFO mapreduce.Job:  map 77% reduce 0%
17/05/09 05:46:15 INFO mapreduce.Job:  map 79% reduce 0%
17/05/09 05:46:18 INFO mapreduce.Job:  map 81% reduce 0%
17/05/09 05:46:21 INFO mapreduce.Job:  map 84% reduce 0%
17/05/09 05:46:24 INFO mapreduce.Job:  map 86% reduce 0%
17/05/09 05:46:27 INFO mapreduce.Job:  map 88% reduce 0%
17/05/09 05:46:30 INFO mapreduce.Job:  map 90% reduce 0%
17/05/09 05:46:33 INFO mapreduce.Job:  map 92% reduce 0%
17/05/09 05:46:35 INFO mapreduce.Job:  map 93% reduce 0%
17/05/09 05:46:36 INFO mapreduce.Job:  map 95% reduce 0%
17/05/09 05:46:39 INFO mapreduce.Job:  map 97% reduce 0%
17/05/09 05:46:42 INFO mapreduce.Job:  map 99% reduce 0%
17/05/09 05:46:45 INFO mapreduce.Job:  map 100% reduce 0%
17/05/09 05:46:45 INFO mapreduce.Job: Job job_1494292583990_0006 completed successfully
17/05/09 05:46:45 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=492380
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=344
		HDFS: Number of bytes written=10485760000
		HDFS: Number of read operations=16
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=8
	Job Counters 
		Launched map tasks=4
		Other local map tasks=4
		Total time spent by all maps in occupied slots (ms)=501298
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=501298
		Total vcore-seconds taken by all map tasks=501298
		Total megabyte-seconds taken by all map tasks=513329152
	Map-Reduce Framework
		Map input records=104857600
		Map output records=104857600
		Input split bytes=344
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=1615
		CPU time spent (ms)=159950
		Physical memory (bytes) snapshot=924684288
		Virtual memory (bytes) snapshot=6269521920
		Total committed heap usage (bytes)=829423616
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=225186913807133164
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=10485760000

real	2m22.451s
user	0m6.899s
sys	0m0.840s


[xiaohu-liu@ip-172-31-7-188 root]$ hadoop fs -ls -h /user/xiaohu-liu/terasort-input
Found 5 items
-rw-r--r--   3 xiaohu-liu supergroup          0 2017-05-09 05:46 /user/xiaohu-liu/terasort-input/_SUCCESS
-rw-r--r--   3 xiaohu-liu supergroup      2.4 G 2017-05-09 05:46 /user/xiaohu-liu/terasort-input/part-m-00000
-rw-r--r--   3 xiaohu-liu supergroup      2.4 G 2017-05-09 05:46 /user/xiaohu-liu/terasort-input/part-m-00001
-rw-r--r--   3 xiaohu-liu supergroup      2.4 G 2017-05-09 05:46 /user/xiaohu-liu/terasort-input/part-m-00002
-rw-r--r--   3 xiaohu-liu supergroup      2.4 G 2017-05-09 05:46 /user/xiaohu-liu/terasort-input/part-m-00003


[xiaohu-liu@ip-172-31-7-188 root]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/xiaohu-liu/terasort-input /user/xiaohu-liu/terasort-output
17/05/09 06:20:01 INFO terasort.TeraSort: starting
17/05/09 06:20:02 INFO input.FileInputFormat: Total input paths to process : 4
Spent 264ms computing base-splits.
Spent 9ms computing TeraScheduler splits.
Computing input splits took 274ms
Sampling 10 splits of 316
Making 8 from 100000 sampled records
Computing parititions took 1084ms
Spent 1361ms computing partitions.
17/05/09 06:20:03 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-0-239/172.31.0.239:8032
17/05/09 06:20:04 INFO mapreduce.JobSubmitter: number of splits:316
17/05/09 06:20:04 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494292583990_0008
17/05/09 06:20:04 INFO impl.YarnClientImpl: Submitted application application_1494292583990_0008
17/05/09 06:20:04 INFO mapreduce.Job: The url to track the job: http://ip-172-31-0-239:8088/proxy/application_1494292583990_0008/
17/05/09 06:20:04 INFO mapreduce.Job: Running job: job_1494292583990_0008
17/05/09 06:20:11 INFO mapreduce.Job: Job job_1494292583990_0008 running in uber mode : false
17/05/09 06:20:11 INFO mapreduce.Job:  map 0% reduce 0%
17/05/09 06:20:19 INFO mapreduce.Job:  map 1% reduce 0%
17/05/09 06:20:23 INFO mapreduce.Job:  map 2% reduce 0%
17/05/09 06:20:26 INFO mapreduce.Job:  map 3% reduce 0%
17/05/09 06:20:33 INFO mapreduce.Job:  map 4% reduce 0%
17/05/09 06:20:34 INFO mapreduce.Job:  map 5% reduce 0%
17/05/09 06:20:37 INFO mapreduce.Job:  map 6% reduce 0%
17/05/09 06:20:45 INFO mapreduce.Job:  map 7% reduce 0%
17/05/09 06:20:46 INFO mapreduce.Job:  map 8% reduce 0%
17/05/09 06:20:47 INFO mapreduce.Job:  map 9% reduce 0%
17/05/09 06:20:54 INFO mapreduce.Job:  map 10% reduce 0%
17/05/09 06:20:56 INFO mapreduce.Job:  map 11% reduce 0%
17/05/09 06:21:01 INFO mapreduce.Job:  map 12% reduce 0%
17/05/09 06:21:06 INFO mapreduce.Job:  map 13% reduce 0%
17/05/09 06:21:08 INFO mapreduce.Job:  map 14% reduce 0%
17/05/09 06:21:15 INFO mapreduce.Job:  map 15% reduce 0%
17/05/09 06:21:16 INFO mapreduce.Job:  map 16% reduce 0%
17/05/09 06:21:22 INFO mapreduce.Job:  map 17% reduce 0%
17/05/09 06:21:25 INFO mapreduce.Job:  map 18% reduce 0%
17/05/09 06:21:27 INFO mapreduce.Job:  map 19% reduce 0%
17/05/09 06:21:33 INFO mapreduce.Job:  map 20% reduce 0%
17/05/09 06:21:36 INFO mapreduce.Job:  map 21% reduce 0%
17/05/09 06:21:37 INFO mapreduce.Job:  map 22% reduce 0%
17/05/09 06:21:43 INFO mapreduce.Job:  map 23% reduce 0%
17/05/09 06:21:47 INFO mapreduce.Job:  map 24% reduce 0%
17/05/09 06:21:50 INFO mapreduce.Job:  map 25% reduce 0%
17/05/09 06:21:56 INFO mapreduce.Job:  map 26% reduce 0%
17/05/09 06:21:57 INFO mapreduce.Job:  map 27% reduce 0%
17/05/09 06:22:03 INFO mapreduce.Job:  map 28% reduce 0%
17/05/09 06:22:06 INFO mapreduce.Job:  map 29% reduce 0%
17/05/09 06:22:10 INFO mapreduce.Job:  map 30% reduce 0%
17/05/09 06:22:14 INFO mapreduce.Job:  map 31% reduce 0%
17/05/09 06:22:18 INFO mapreduce.Job:  map 32% reduce 0%
17/05/09 06:22:22 INFO mapreduce.Job:  map 33% reduce 0%
17/05/09 06:22:26 INFO mapreduce.Job:  map 34% reduce 0%
17/05/09 06:22:30 INFO mapreduce.Job:  map 35% reduce 0%
17/05/09 06:22:33 INFO mapreduce.Job:  map 36% reduce 0%
17/05/09 06:22:38 INFO mapreduce.Job:  map 37% reduce 0%
17/05/09 06:22:39 INFO mapreduce.Job:  map 38% reduce 0%
17/05/09 06:22:46 INFO mapreduce.Job:  map 39% reduce 0%
17/05/09 06:22:47 INFO mapreduce.Job:  map 40% reduce 0%
17/05/09 06:22:52 INFO mapreduce.Job:  map 41% reduce 0%
17/05/09 06:22:56 INFO mapreduce.Job:  map 42% reduce 0%
17/05/09 06:22:59 INFO mapreduce.Job:  map 43% reduce 0%
17/05/09 06:23:03 INFO mapreduce.Job:  map 44% reduce 0%
17/05/09 06:23:06 INFO mapreduce.Job:  map 45% reduce 0%
17/05/09 06:23:10 INFO mapreduce.Job:  map 46% reduce 0%
17/05/09 06:23:13 INFO mapreduce.Job:  map 47% reduce 0%
17/05/09 06:23:19 INFO mapreduce.Job:  map 48% reduce 0%
17/05/09 06:23:20 INFO mapreduce.Job:  map 49% reduce 0%
17/05/09 06:23:26 INFO mapreduce.Job:  map 50% reduce 0%
17/05/09 06:23:28 INFO mapreduce.Job:  map 51% reduce 0%
17/05/09 06:23:34 INFO mapreduce.Job:  map 52% reduce 0%
17/05/09 06:23:35 INFO mapreduce.Job:  map 53% reduce 0%
17/05/09 06:23:41 INFO mapreduce.Job:  map 54% reduce 0%
17/05/09 06:23:45 INFO mapreduce.Job:  map 55% reduce 0%
17/05/09 06:23:49 INFO mapreduce.Job:  map 56% reduce 0%
17/05/09 06:23:51 INFO mapreduce.Job:  map 57% reduce 0%
17/05/09 06:23:55 INFO mapreduce.Job:  map 58% reduce 0%
17/05/09 06:23:58 INFO mapreduce.Job:  map 59% reduce 0%
17/05/09 06:24:04 INFO mapreduce.Job:  map 60% reduce 0%
17/05/09 06:24:07 INFO mapreduce.Job:  map 61% reduce 0%
17/05/09 06:24:08 INFO mapreduce.Job:  map 62% reduce 0%
17/05/09 06:24:14 INFO mapreduce.Job:  map 63% reduce 0%
17/05/09 06:24:17 INFO mapreduce.Job:  map 64% reduce 0%
17/05/09 06:24:22 INFO mapreduce.Job:  map 65% reduce 0%
17/05/09 06:24:24 INFO mapreduce.Job:  map 66% reduce 0%
17/05/09 06:24:29 INFO mapreduce.Job:  map 67% reduce 0%
17/05/09 06:24:34 INFO mapreduce.Job:  map 68% reduce 0%
17/05/09 06:24:36 INFO mapreduce.Job:  map 69% reduce 0%
17/05/09 06:24:39 INFO mapreduce.Job:  map 70% reduce 0%
17/05/09 06:24:44 INFO mapreduce.Job:  map 71% reduce 0%
17/05/09 06:24:46 INFO mapreduce.Job:  map 72% reduce 0%
17/05/09 06:24:53 INFO mapreduce.Job:  map 73% reduce 0%
17/05/09 06:24:56 INFO mapreduce.Job:  map 74% reduce 0%
17/05/09 06:24:58 INFO mapreduce.Job:  map 75% reduce 0%
17/05/09 06:25:03 INFO mapreduce.Job:  map 76% reduce 0%
17/05/09 06:25:06 INFO mapreduce.Job:  map 77% reduce 0%
17/05/09 06:25:10 INFO mapreduce.Job:  map 78% reduce 0%
17/05/09 06:25:17 INFO mapreduce.Job:  map 79% reduce 0%
17/05/09 06:25:18 INFO mapreduce.Job:  map 80% reduce 0%
17/05/09 06:25:22 INFO mapreduce.Job:  map 81% reduce 0%
17/05/09 06:25:25 INFO mapreduce.Job:  map 82% reduce 0%
17/05/09 06:25:30 INFO mapreduce.Job:  map 83% reduce 0%
17/05/09 06:25:35 INFO mapreduce.Job:  map 83% reduce 2%
17/05/09 06:25:38 INFO mapreduce.Job:  map 83% reduce 4%
17/05/09 06:25:39 INFO mapreduce.Job:  map 84% reduce 4%
17/05/09 06:25:40 INFO mapreduce.Job:  map 84% reduce 7%
17/05/09 06:25:41 INFO mapreduce.Job:  map 84% reduce 10%
17/05/09 06:25:44 INFO mapreduce.Job:  map 84% reduce 12%
17/05/09 06:25:46 INFO mapreduce.Job:  map 85% reduce 13%
17/05/09 06:25:50 INFO mapreduce.Job:  map 85% reduce 14%
17/05/09 06:25:53 INFO mapreduce.Job:  map 86% reduce 14%
17/05/09 06:25:59 INFO mapreduce.Job:  map 87% reduce 14%
17/05/09 06:26:06 INFO mapreduce.Job:  map 88% reduce 14%
17/05/09 06:26:07 INFO mapreduce.Job:  map 88% reduce 15%
17/05/09 06:26:13 INFO mapreduce.Job:  map 89% reduce 15%
17/05/09 06:26:20 INFO mapreduce.Job:  map 90% reduce 15%
17/05/09 06:26:27 INFO mapreduce.Job:  map 91% reduce 15%
17/05/09 06:26:38 INFO mapreduce.Job:  map 92% reduce 15%
17/05/09 06:26:45 INFO mapreduce.Job:  map 93% reduce 15%
17/05/09 06:26:50 INFO mapreduce.Job:  map 93% reduce 16%
17/05/09 06:26:52 INFO mapreduce.Job:  map 94% reduce 16%
17/05/09 06:26:58 INFO mapreduce.Job:  map 95% reduce 16%
17/05/09 06:27:05 INFO mapreduce.Job:  map 96% reduce 16%
17/05/09 06:27:11 INFO mapreduce.Job:  map 97% reduce 16%
17/05/09 06:27:22 INFO mapreduce.Job:  map 98% reduce 16%
17/05/09 06:27:28 INFO mapreduce.Job:  map 99% reduce 16%
17/05/09 06:27:31 INFO mapreduce.Job:  map 99% reduce 17%
17/05/09 06:27:34 INFO mapreduce.Job:  map 100% reduce 17%
17/05/09 06:27:35 INFO mapreduce.Job:  map 100% reduce 18%
17/05/09 06:27:36 INFO mapreduce.Job:  map 100% reduce 19%
17/05/09 06:27:37 INFO mapreduce.Job:  map 100% reduce 22%
17/05/09 06:27:38 INFO mapreduce.Job:  map 100% reduce 29%
17/05/09 06:27:39 INFO mapreduce.Job:  map 100% reduce 33%
17/05/09 06:27:40 INFO mapreduce.Job:  map 100% reduce 34%
17/05/09 06:27:41 INFO mapreduce.Job:  map 100% reduce 36%
17/05/09 06:27:43 INFO mapreduce.Job:  map 100% reduce 37%
17/05/09 06:27:44 INFO mapreduce.Job:  map 100% reduce 39%
17/05/09 06:27:45 INFO mapreduce.Job:  map 100% reduce 45%
17/05/09 06:27:47 INFO mapreduce.Job:  map 100% reduce 46%
17/05/09 06:27:48 INFO mapreduce.Job:  map 100% reduce 48%
17/05/09 06:27:49 INFO mapreduce.Job:  map 100% reduce 49%
17/05/09 06:27:50 INFO mapreduce.Job:  map 100% reduce 51%
17/05/09 06:27:51 INFO mapreduce.Job:  map 100% reduce 52%
17/05/09 06:27:52 INFO mapreduce.Job:  map 100% reduce 53%
17/05/09 06:27:54 INFO mapreduce.Job:  map 100% reduce 60%
17/05/09 06:27:55 INFO mapreduce.Job:  map 100% reduce 61%
17/05/09 06:27:56 INFO mapreduce.Job:  map 100% reduce 63%
17/05/09 06:27:57 INFO mapreduce.Job:  map 100% reduce 68%
17/05/09 06:27:59 INFO mapreduce.Job:  map 100% reduce 72%
17/05/09 06:28:00 INFO mapreduce.Job:  map 100% reduce 74%
17/05/09 06:28:02 INFO mapreduce.Job:  map 100% reduce 75%
17/05/09 06:28:03 INFO mapreduce.Job:  map 100% reduce 77%
17/05/09 06:28:05 INFO mapreduce.Job:  map 100% reduce 78%
17/05/09 06:28:06 INFO mapreduce.Job:  map 100% reduce 80%
17/05/09 06:28:09 INFO mapreduce.Job:  map 100% reduce 83%
17/05/09 06:28:10 INFO mapreduce.Job:  map 100% reduce 86%
17/05/09 06:28:11 INFO mapreduce.Job:  map 100% reduce 87%
17/05/09 06:28:12 INFO mapreduce.Job:  map 100% reduce 88%
17/05/09 06:28:13 INFO mapreduce.Job:  map 100% reduce 89%
17/05/09 06:28:16 INFO mapreduce.Job:  map 100% reduce 90%
17/05/09 06:28:17 INFO mapreduce.Job:  map 100% reduce 91%
17/05/09 06:28:19 INFO mapreduce.Job:  map 100% reduce 95%
17/05/09 06:28:20 INFO mapreduce.Job:  map 100% reduce 96%
17/05/09 06:28:25 INFO mapreduce.Job:  map 100% reduce 97%
17/05/09 06:28:28 INFO mapreduce.Job:  map 100% reduce 98%
17/05/09 06:28:31 INFO mapreduce.Job:  map 100% reduce 99%
17/05/09 06:28:34 INFO mapreduce.Job:  map 100% reduce 100%
17/05/09 06:28:36 INFO mapreduce.Job: Job job_1494292583990_0008 completed successfully
17/05/09 06:28:37 INFO mapreduce.Job: Counters: 49
	File System Counters
		FILE: Number of bytes read=4698340817
		FILE: Number of bytes written=9326007194
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=10485802976
		HDFS: Number of bytes written=10485760000
		HDFS: Number of read operations=972
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=16
	Job Counters 
		Launched map tasks=316
		Launched reduce tasks=8
		Data-local map tasks=316
		Total time spent by all maps in occupied slots (ms)=2193674
		Total time spent by all reduces in occupied slots (ms)=789453
		Total time spent by all map tasks (ms)=2193674
		Total time spent by all reduce tasks (ms)=789453
		Total vcore-seconds taken by all map tasks=2193674
		Total vcore-seconds taken by all reduce tasks=789453
		Total megabyte-seconds taken by all map tasks=2246322176
		Total megabyte-seconds taken by all reduce tasks=808399872
	Map-Reduce Framework
		Map input records=104857600
		Map output records=104857600
		Map output bytes=10695475200
		Map output materialized bytes=4587294679
		Input split bytes=42976
		Combine input records=0
		Combine output records=0
		Reduce input groups=104857600
		Reduce shuffle bytes=4587294679
		Reduce input records=104857600
		Reduce output records=104857600
		Spilled Records=209715200
		Shuffled Maps =2528
		Failed Shuffles=0
		Merged Map outputs=2528
		GC time elapsed (ms)=29001
		CPU time spent (ms)=1462030
		Physical memory (bytes) snapshot=152782577664
		Virtual memory (bytes) snapshot=507274440704
		Total committed heap usage (bytes)=184561434624
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=10485760000
	File Output Format Counters 
		Bytes Written=10485760000
17/05/09 06:28:37 INFO terasort.TeraSort: done

real	8m37.187s
user	0m10.495s
sys	0m1.134s

[xiaohu-liu@ip-172-31-7-188 root]$ hadoop fs -ls -h /user/xiaohu-liu/terasort-output
Found 10 items
-rw-r--r--   1 xiaohu-liu supergroup          0 2017-05-09 06:28 /user/xiaohu-liu/terasort-output/_SUCCESS
-rw-r--r--  10 xiaohu-liu supergroup         77 2017-05-09 06:20 /user/xiaohu-liu/terasort-output/_partition.lst
-rw-r--r--   1 xiaohu-liu supergroup      1.2 G 2017-05-09 06:28 /user/xiaohu-liu/terasort-output/part-r-00000
-rw-r--r--   1 xiaohu-liu supergroup      1.2 G 2017-05-09 06:27 /user/xiaohu-liu/terasort-output/part-r-00001
-rw-r--r--   1 xiaohu-liu supergroup      1.2 G 2017-05-09 06:27 /user/xiaohu-liu/terasort-output/part-r-00002
-rw-r--r--   1 xiaohu-liu supergroup      1.2 G 2017-05-09 06:28 /user/xiaohu-liu/terasort-output/part-r-00003
-rw-r--r--   1 xiaohu-liu supergroup      1.2 G 2017-05-09 06:28 /user/xiaohu-liu/terasort-output/part-r-00004
-rw-r--r--   1 xiaohu-liu supergroup      1.2 G 2017-05-09 06:28 /user/xiaohu-liu/terasort-output/part-r-00005
-rw-r--r--   1 xiaohu-liu supergroup      1.2 G 2017-05-09 06:28 /user/xiaohu-liu/terasort-output/part-r-00006
-rw-r--r--   1 xiaohu-liu supergroup      1.2 G 2017-05-09 06:28 /user/xiaohu-liu/terasort-output/part-r-00007
```
