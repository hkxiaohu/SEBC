### Verify user privileges
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

### kinit as george, login to beeline, and use SHOW TABLES;
```
[root@ip-172-31-7-188 etc]# su george
[george@ip-172-31-7-188 etc]$ kinit george
Password for george@XIAOHU-LIU.CN: 
[george@ip-172-31-7-188 etc]$ beeline
Beeline version 1.1.0-cdh5.9.2 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-7-206:10000/default;principal=hive/ip-172-31-7-206@XIAOHU-LIU.CN
scan complete in 2ms
Connecting to jdbc:hive2://ip-172-31-7-206:10000/default;principal=hive/ip-172-31-7-206@XIAOHU-LIU.CN
Connected to: Apache Hive (version 1.1.0-cdh5.9.2)
Driver: Hive JDBC (version 1.1.0-cdh5.9.2)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-7-206:10000/default> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20170510105353_55ddf486-e72f-42b5-a2b8-e6eff770104b): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170510105353_55ddf486-e72f-42b5-a2b8-e6eff770104b); Time taken: 0.071 seconds
INFO  : Executing command(queryId=hive_20170510105353_55ddf486-e72f-42b5-a2b8-e6eff770104b): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510105353_55ddf486-e72f-42b5-a2b8-e6eff770104b); Time taken: 0.143 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.336 seconds)
0: jdbc:hive2://ip-172-31-7-206:10000/default> !quit
```


### kinit as ferdinand, login to beeline, and use SHOW TABLES
```
[root@ip-172-31-7-188 etc]# su ferdinand
[ferdinand@ip-172-31-7-188 etc]$ kinit ferdinand
Password for ferdinand@XIAOHU-LIU.CN: 
[ferdinand@ip-172-31-7-188 etc]$ beeline
Beeline version 1.1.0-cdh5.9.2 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-7-206:10000/default;principal=hive/ip-172-31-7-206@XIAOHU-LIU.CN
scan complete in 2ms
Connecting to jdbc:hive2://ip-172-31-7-206:10000/default;principal=hive/ip-172-31-7-206@XIAOHU-LIU.CN
Connected to: Apache Hive (version 1.1.0-cdh5.9.2)
Driver: Hive JDBC (version 1.1.0-cdh5.9.2)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-7-206:10000/default> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20170510105454_62cd25d4-0593-445d-a4af-3fe21013d179): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170510105454_62cd25d4-0593-445d-a4af-3fe21013d179); Time taken: 0.072 seconds
INFO  : Executing command(queryId=hive_20170510105454_62cd25d4-0593-445d-a4af-3fe21013d179): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510105454_62cd25d4-0593-445d-a4af-3fe21013d179); Time taken: 0.134 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| sample_07  |
+------------+--+
1 row selected (0.307 seconds)
0: jdbc:hive2://ip-172-31-7-206:10000/default> !quit
```








