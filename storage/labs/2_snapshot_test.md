Create a precious directory in HDFS; copy the ZIP course file into it.
```
[hdfs@ip-172-31-7-188 tmp]$ hadoop fs -mkdir /precious
[hdfs@ip-172-31-7-188 tmp]$ hadoop fs -put SEBC-Shanghai.zip /precious
[hdfs@ip-172-31-7-188 tmp]$ hadoop fs -ls /precious
Found 1 items
-rw-r--r--   3 hdfs supergroup     474957 2017-05-09 06:55 /precious/SEBC-Shanghai.zip
```

Enable snapshots for precious
```
[hdfs@ip-172-31-7-188 tmp]$ hdfs dfsadmin -allowSnapshot /precious
Allowing snaphot on /precious succeeded
```

Create a snapshot called sebc-hdfs-test
```
[hdfs@ip-172-31-7-188 tmp]$ hadoop fs -createSnapshot /precious sebc-hdfs-test
Created snapshot /precious/.snapshot/sebc-hdfs-test
```

Delete the directory
```
[hdfs@ip-172-31-7-188 tmp]$ hadoop fs -rm -r -skipTrash /precious
rm: The directory /precious cannot be deleted since /precious is snapshottable and already has snapshots
```
Delete the ZIP file
```
[hdfs@ip-172-31-7-188 tmp]$ hadoop fs -rm -r -skipTrash /precious/SEBC-Shanghai.zip
Deleted /precious/SEBC-Shanghai.zip
```

Restore the deleted file
```
[hdfs@ip-172-31-7-188 tmp]$ hadoop fs -cp /precious/.snapshot/sebc-hdfs-test/SEBC-Shanghai.zip /precious/
[hdfs@ip-172-31-7-188 tmp]$ hadoop fs -ls /precious
Found 1 items
-rw-r--r--   3 hdfs supergroup     474957 2017-05-09 07:08 /precious/SEBC-Shanghai.zip
```
