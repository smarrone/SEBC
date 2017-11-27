```
[reilly@ip-172-31-47-134 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -Ddfs.block.size=33554432 -Dmapreduce.job.maps=12 -Dmapreduce.map.memory.mb=1024 65536000 /user/reilly/tgen
```
```
17/11/03 06:03:15 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-39-184.eu-central-1.compute.internal/172.31.39.184:8032
17/11/03 06:03:16 INFO terasort.TeraSort: Generating 65536000 using 12
17/11/03 06:03:16 INFO mapreduce.JobSubmitter: number of splits:12
17/11/03 06:03:16 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/11/03 06:03:16 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1509702219130_0001
17/11/03 06:03:17 INFO impl.YarnClientImpl: Submitted application application_1509702219130_0001
17/11/03 06:03:17 INFO mapreduce.Job: The url to track the job: http://ip-172-31-39-184.eu-central-1.compute.internal:8088/proxy/application_1509702219130_0001/
17/11/03 06:03:17 INFO mapreduce.Job: Running job: job_1509702219130_0001
17/11/03 06:03:23 INFO mapreduce.Job: Job job_1509702219130_0001 running in uber mode : false
17/11/03 06:03:23 INFO mapreduce.Job:  map 0% reduce 0%
17/11/03 06:03:35 INFO mapreduce.Job:  map 8% reduce 0%
17/11/03 06:03:37 INFO mapreduce.Job:  map 19% reduce 0%
17/11/03 06:03:38 INFO mapreduce.Job:  map 21% reduce 0%
17/11/03 06:03:39 INFO mapreduce.Job:  map 22% reduce 0%
17/11/03 06:03:40 INFO mapreduce.Job:  map 25% reduce 0%
17/11/03 06:03:41 INFO mapreduce.Job:  map 26% reduce 0%
17/11/03 06:03:42 INFO mapreduce.Job:  map 29% reduce 0%
17/11/03 06:03:43 INFO mapreduce.Job:  map 31% reduce 0%
17/11/03 06:03:46 INFO mapreduce.Job:  map 32% reduce 0%
17/11/03 06:03:47 INFO mapreduce.Job:  map 33% reduce 0%
17/11/03 06:03:51 INFO mapreduce.Job:  map 36% reduce 0%
17/11/03 06:03:52 INFO mapreduce.Job:  map 37% reduce 0%
17/11/03 06:03:53 INFO mapreduce.Job:  map 40% reduce 0%
17/11/03 06:03:54 INFO mapreduce.Job:  map 42% reduce 0%
17/11/03 06:03:56 INFO mapreduce.Job:  map 43% reduce 0%
17/11/03 06:04:04 INFO mapreduce.Job:  map 44% reduce 0%
17/11/03 06:04:05 INFO mapreduce.Job:  map 46% reduce 0%
17/11/03 06:04:06 INFO mapreduce.Job:  map 49% reduce 0%
17/11/03 06:04:07 INFO mapreduce.Job:  map 51% reduce 0%
17/11/03 06:04:08 INFO mapreduce.Job:  map 54% reduce 0%
17/11/03 06:04:12 INFO mapreduce.Job:  map 58% reduce 0%
17/11/03 06:04:17 INFO mapreduce.Job:  map 60% reduce 0%
17/11/03 06:04:18 INFO mapreduce.Job:  map 61% reduce 0%
17/11/03 06:04:20 INFO mapreduce.Job:  map 63% reduce 0%
17/11/03 06:04:23 INFO mapreduce.Job:  map 64% reduce 0%
17/11/03 06:04:24 INFO mapreduce.Job:  map 65% reduce 0%
17/11/03 06:04:26 INFO mapreduce.Job:  map 68% reduce 0%
17/11/03 06:04:27 INFO mapreduce.Job:  map 69% reduce 0%
17/11/03 06:04:29 INFO mapreduce.Job:  map 73% reduce 0%
17/11/03 06:04:30 INFO mapreduce.Job:  map 74% reduce 0%
17/11/03 06:04:38 INFO mapreduce.Job:  map 82% reduce 0%
17/11/03 06:04:39 INFO mapreduce.Job:  map 83% reduce 0%
17/11/03 06:04:41 INFO mapreduce.Job:  map 86% reduce 0%
17/11/03 06:04:44 INFO mapreduce.Job:  map 87% reduce 0%
17/11/03 06:04:45 INFO mapreduce.Job:  map 88% reduce 0%
17/11/03 06:04:47 INFO mapreduce.Job:  map 89% reduce 0%
17/11/03 06:04:48 INFO mapreduce.Job:  map 90% reduce 0%
17/11/03 06:04:50 INFO mapreduce.Job:  map 93% reduce 0%
17/11/03 06:04:57 INFO mapreduce.Job:  map 96% reduce 0%
17/11/03 06:04:59 INFO mapreduce.Job:  map 99% reduce 0%
17/11/03 06:05:02 INFO mapreduce.Job:  map 100% reduce 0%
17/11/03 06:05:02 INFO mapreduce.Job: Job job_1509702219130_0001 completed successfully
17/11/03 06:05:02 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=1469870
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=1025
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=48
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=24
        Job Counters
                Launched map tasks=12
                Other local map tasks=12
                Total time spent by all maps in occupied slots (ms)=516876
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=516876
                Total vcore-seconds taken by all map tasks=516876
                Total megabyte-seconds taken by all map tasks=529281024
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=1025
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=1886
                CPU time spent (ms)=148220
                Physical memory (bytes) snapshot=4054921216
                Virtual memory (bytes) snapshot=18955956224
                Total committed heap usage (bytes)=4348444672
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000

real    1m49.054s
user    0m6.026s
sys     0m0.276s
```


```
[reilly@ip-172-31-47-134 ~]$ hdfs dfs -ls /user/reilly/tgen
Found 13 items
-rw-r--r--   3 reilly reilly          0 2017-11-03 06:05 /user/reilly/tgen/_SUCCESS
-rw-r--r--   3 reilly reilly  546133400 2017-11-03 06:04 /user/reilly/tgen/part-m-00000
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:04 /user/reilly/tgen/part-m-00001
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:04 /user/reilly/tgen/part-m-00002
-rw-r--r--   3 reilly reilly  546133400 2017-11-03 06:04 /user/reilly/tgen/part-m-00003
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:04 /user/reilly/tgen/part-m-00004
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:03 /user/reilly/tgen/part-m-00005
-rw-r--r--   3 reilly reilly  546133400 2017-11-03 06:04 /user/reilly/tgen/part-m-00006
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:05 /user/reilly/tgen/part-m-00007
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:04 /user/reilly/tgen/part-m-00008
-rw-r--r--   3 reilly reilly  546133400 2017-11-03 06:05 /user/reilly/tgen/part-m-00009
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:05 /user/reilly/tgen/part-m-00010
-rw-r--r--   3 reilly reilly  546133300 2017-11-03 06:04 /user/reilly/tgen/part-m-00011
```

```
[reilly@ip-172-31-47-134 ~]$ hadoop fsck -blocks /user/reilly/tgen
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.

Connecting to namenode via http://ip-172-31-39-17.eu-central-1.compute.internal:50070
FSCK started by reilly (auth:SIMPLE) from /172.31.47.134 for path /user/reilly/tgen at Fri Nov 03 06:06:43 EDT 2017
.............Status: HEALTHY
 Total size:    6553600000 B
 Total dirs:    1
 Total files:   13
 Total symlinks:                0
 Total blocks (validated):      204 (avg. block size 32125490 B)
 Minimally replicated blocks:   204 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          5
 Number of racks:               1
FSCK ended at Fri Nov 03 06:06:43 EDT 2017 in 10 milliseconds


The filesystem under path '/user/reilly/tgen' is HEALTHY
```
