```
[xiaohu-liu@ip-172-31-7-188 etc]$ beeline
Beeline version 1.1.0-cdh5.9.2 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-7-206:10000/default;principal=hive/ip-172-31-7-206@XIAOHU-LIU.CN
scan complete in 2ms
Connecting to jdbc:hive2://ip-172-31-7-206:10000/default;principal=hive/ip-172-31-7-206@XIAOHU-LIU.CN
Connected to: Apache Hive (version 1.1.0-cdh5.9.2)
Driver: Hive JDBC (version 1.1.0-cdh5.9.2)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-7-206:10000/default> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20170510103939_4667e0e5-4f21-4709-afd3-af9f33ab8ddf): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170510103939_4667e0e5-4f21-4709-afd3-af9f33ab8ddf); Time taken: 0.744 seconds
INFO  : Executing command(queryId=hive_20170510103939_4667e0e5-4f21-4709-afd3-af9f33ab8ddf): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510103939_4667e0e5-4f21-4709-afd3-af9f33ab8ddf); Time taken: 0.419 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (2.521 seconds)
0: jdbc:hive2://ip-172-31-7-206:10000/default>
```
