```
[chen@ip-172-31-7-7 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar pi 100 100000
Number of Maps  = 100
Samples per Map = 100000
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Wrote input for Map #5
Wrote input for Map #6
Wrote input for Map #7
Wrote input for Map #8
Wrote input for Map #9
Wrote input for Map #10
Wrote input for Map #11
Wrote input for Map #12
Wrote input for Map #13
Wrote input for Map #14
Wrote input for Map #15
Wrote input for Map #16
Wrote input for Map #17
Wrote input for Map #18
Wrote input for Map #19
Wrote input for Map #20
Wrote input for Map #21
Wrote input for Map #22
Wrote input for Map #23
Wrote input for Map #24
Wrote input for Map #25
Wrote input for Map #26
Wrote input for Map #27
Wrote input for Map #28
Wrote input for Map #29
Wrote input for Map #30
Wrote input for Map #31
Wrote input for Map #32
Wrote input for Map #33
Wrote input for Map #34
Wrote input for Map #35
Wrote input for Map #36
Wrote input for Map #37
Wrote input for Map #38
Wrote input for Map #39
Wrote input for Map #40
Wrote input for Map #41
Wrote input for Map #42
Wrote input for Map #43
Wrote input for Map #44
Wrote input for Map #45
Wrote input for Map #46
Wrote input for Map #47
Wrote input for Map #48
Wrote input for Map #49
Wrote input for Map #50
Wrote input for Map #51
Wrote input for Map #52
Wrote input for Map #53
Wrote input for Map #54
Wrote input for Map #55
Wrote input for Map #56
Wrote input for Map #57
Wrote input for Map #58
Wrote input for Map #59
Wrote input for Map #60
Wrote input for Map #61
Wrote input for Map #62
Wrote input for Map #63
Wrote input for Map #64
Wrote input for Map #65
Wrote input for Map #66
Wrote input for Map #67
Wrote input for Map #68
Wrote input for Map #69
Wrote input for Map #70
Wrote input for Map #71
Wrote input for Map #72
Wrote input for Map #73
Wrote input for Map #74
Wrote input for Map #75
Wrote input for Map #76
Wrote input for Map #77
Wrote input for Map #78
Wrote input for Map #79
Wrote input for Map #80
Wrote input for Map #81
Wrote input for Map #82
Wrote input for Map #83
Wrote input for Map #84
Wrote input for Map #85
Wrote input for Map #86
Wrote input for Map #87
Wrote input for Map #88
Wrote input for Map #89
Wrote input for Map #90
Wrote input for Map #91
Wrote input for Map #92
Wrote input for Map #93
Wrote input for Map #94
Wrote input for Map #95
Wrote input for Map #96
Wrote input for Map #97
Wrote input for Map #98
Wrote input for Map #99
Starting Job
17/05/12 03:00:58 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-3-172/172.31.3.172:8032
17/05/12 03:00:58 INFO hdfs.DFSClient: Created token for chen: HDFS_DELEGATION_TOKEN owner=chen@XIAOHU-LIU.CN, renewer=yarn, realUser=, issueDate=1494558058899, maxDate=1495162858899, sequenceNumber=2, masterKeyId=2 on 172.31.4.25:8020
17/05/12 03:00:58 INFO security.TokenCache: Got dt for hdfs://ip-172-31-4-25:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.4.25:8020, Ident: (token for chen: HDFS_DELEGATION_TOKEN owner=chen@XIAOHU-LIU.CN, renewer=yarn, realUser=, issueDate=1494558058899, maxDate=1495162858899, sequenceNumber=2, masterKeyId=2)
17/05/12 03:00:59 INFO input.FileInputFormat: Total input paths to process : 100
17/05/12 03:00:59 INFO mapreduce.JobSubmitter: number of splits:100
17/05/12 03:00:59 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494557335908_0002
17/05/12 03:00:59 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.4.25:8020, Ident: (token for chen: HDFS_DELEGATION_TOKEN owner=chen@XIAOHU-LIU.CN, renewer=yarn, realUser=, issueDate=1494558058899, maxDate=1495162858899, sequenceNumber=2, masterKeyId=2)
17/05/12 03:00:59 INFO impl.YarnClientImpl: Submitted application application_1494557335908_0002
17/05/12 03:00:59 INFO mapreduce.Job: The url to track the job: http://ip-172-31-3-172:8088/proxy/application_1494557335908_0002/
17/05/12 03:00:59 INFO mapreduce.Job: Running job: job_1494557335908_0002
17/05/12 03:01:08 INFO mapreduce.Job: Job job_1494557335908_0002 running in uber mode : false
17/05/12 03:01:08 INFO mapreduce.Job:  map 0% reduce 0%
17/05/12 03:01:16 INFO mapreduce.Job:  map 2% reduce 0%
17/05/12 03:01:17 INFO mapreduce.Job:  map 4% reduce 0%
17/05/12 03:01:21 INFO mapreduce.Job:  map 8% reduce 0%
17/05/12 03:01:25 INFO mapreduce.Job:  map 12% reduce 0%
17/05/12 03:01:29 INFO mapreduce.Job:  map 16% reduce 0%
17/05/12 03:01:33 INFO mapreduce.Job:  map 20% reduce 0%
17/05/12 03:01:37 INFO mapreduce.Job:  map 24% reduce 0%
17/05/12 03:01:41 INFO mapreduce.Job:  map 28% reduce 0%
17/05/12 03:01:45 INFO mapreduce.Job:  map 32% reduce 0%
17/05/12 03:01:49 INFO mapreduce.Job:  map 36% reduce 0%
17/05/12 03:01:53 INFO mapreduce.Job:  map 40% reduce 0%
`17/05/12 03:01:57 INFO mapreduce.Job:  map 44% reduce 0%
17/05/12 03:02:01 INFO mapreduce.Job:  map 48% reduce 0%
17/05/12 03:02:05 INFO mapreduce.Job:  map 52% reduce 0%
17/05/12 03:02:09 INFO mapreduce.Job:  map 56% reduce 0%
17/05/12 03:02:13 INFO mapreduce.Job:  map 60% reduce 0%
17/05/12 03:02:17 INFO mapreduce.Job:  map 63% reduce 0%
17/05/12 03:02:18 INFO mapreduce.Job:  map 64% reduce 0%
17/05/12 03:02:21 INFO mapreduce.Job:  map 67% reduce 0%
17/05/12 03:02:22 INFO mapreduce.Job:  map 68% reduce 0%
17/05/12 03:02:25 INFO mapreduce.Job:  map 71% reduce 0%
17/05/12 03:02:26 INFO mapreduce.Job:  map 72% reduce 0%
17/05/12 03:02:29 INFO mapreduce.Job:  map 75% reduce 0%
17/05/12 03:02:30 INFO mapreduce.Job:  map 76% reduce 0%
17/05/12 03:02:33 INFO mapreduce.Job:  map 79% reduce 0%
17/05/12 03:02:35 INFO mapreduce.Job:  map 80% reduce 0%
17/05/12 03:02:37 INFO mapreduce.Job:  map 83% reduce 0%
17/05/12 03:02:39 INFO mapreduce.Job:  map 84% reduce 0%
17/05/12 03:02:41 INFO mapreduce.Job:  map 86% reduce 0%
17/05/12 03:02:42 INFO mapreduce.Job:  map 87% reduce 0%
17/05/12 03:02:43 INFO mapreduce.Job:  map 88% reduce 0%
17/05/12 03:02:45 INFO mapreduce.Job:  map 89% reduce 0%
17/05/12 03:02:46 INFO mapreduce.Job:  map 90% reduce 0%
17/05/12 03:02:47 INFO mapreduce.Job:  map 91% reduce 0%
17/05/12 03:02:49 INFO mapreduce.Job:  map 92% reduce 0%
17/05/12 03:02:50 INFO mapreduce.Job:  map 93% reduce 31%
17/05/12 03:02:51 INFO mapreduce.Job:  map 94% reduce 31%
17/05/12 03:02:53 INFO mapreduce.Job:  map 95% reduce 31%
17/05/12 03:02:54 INFO mapreduce.Job:  map 96% reduce 31%
17/05/12 03:02:55 INFO mapreduce.Job:  map 97% reduce 31%
17/05/12 03:02:56 INFO mapreduce.Job:  map 97% reduce 32%
17/05/12 03:02:57 INFO mapreduce.Job:  map 98% reduce 32%
17/05/12 03:02:58 INFO mapreduce.Job:  map 99% reduce 32%
17/05/12 03:02:59 INFO mapreduce.Job:  map 100% reduce 33%
17/05/12 03:03:00 INFO mapreduce.Job:  map 100% reduce 100%
17/05/12 03:03:00 INFO mapreduce.Job: Job job_1494557335908_0002 completed successfully
17/05/12 03:03:00 INFO mapreduce.Job: Counters: 50
	File System Counters
		FILE: Number of bytes read=647
		FILE: Number of bytes written=12512123
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=26990
		HDFS: Number of bytes written=215
		HDFS: Number of read operations=403
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=3
	Job Counters 
		Launched map tasks=100
		Launched reduce tasks=1
		Data-local map tasks=98
		Rack-local map tasks=2
		Total time spent by all maps in occupied slots (ms)=333286
		Total time spent by all reduces in occupied slots (ms)=18263
		Total time spent by all map tasks (ms)=333286
		Total time spent by all reduce tasks (ms)=18263
		Total vcore-seconds taken by all map tasks=333286
		Total vcore-seconds taken by all reduce tasks=18263
		Total megabyte-seconds taken by all map tasks=341284864
		Total megabyte-seconds taken by all reduce tasks=18701312
	Map-Reduce Framework
		Map input records=100
		Map output records=200
		Map output bytes=1800
		Map output materialized bytes=3500
		Input split bytes=15190
		Combine input records=0
		Combine output records=0
		Reduce input groups=2
		Reduce shuffle bytes=3500
		Reduce input records=200
		Reduce output records=0
		Spilled Records=400
		Shuffled Maps =100
		Failed Shuffles=0
		Merged Map outputs=100
		GC time elapsed (ms)=2142
		CPU time spent (ms)=70310
		Physical memory (bytes) snapshot=45470691328
		Virtual memory (bytes) snapshot=159811817472
		Total committed heap usage (bytes)=51847888896
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=11800
	File Output Format Counters 
		Bytes Written=97
Job Finished in 122.021 seconds
Estimated value of Pi is 3.14158440000000000000

real	2m6.571s
user	0m5.636s
sys	0m0.826s
```
