### Add the first line of the server's log
```
[root@ip-172-31-7-7 ~]# head -n 1 /var/log/cloudera-scm-server/cloudera-scm-server.log 
2017-05-12 01:52:42,200 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -Dcmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.awt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.11.0 (#101 built by jenkins on 20170412-1249 git: 70cb1442626406432a6e7af5bdf206a384ca3f98)

```


### The log record that contains the phrase "Started Jetty server"
```
[root@ip-172-31-7-7 ~]# cat /var/log/cloudera-scm-server/cloudera-scm-server.log | grep "Started Jetty server"
2017-05-12 01:54:06,803 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.

```
