```
[frankola@ip-172-31-39-17 ~]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar pi 50 100
```
```
Number of Maps  = 50
Samples per Map = 100
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
Starting Job
17/11/03 06:56:30 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-39-184.eu-central-1.compute.internal/172.31.39.184:8032
17/11/03 06:56:30 INFO hdfs.DFSClient: Created token for frankola: HDFS_DELEGATION_TOKEN owner=frankola@SMARRONE.FNG, renewer=yarn, realUser=, issueDate=1509706590224, maxDate=1510311390224, sequenceNumber=2, masterKeyId=2 on 172.31.39.17:8020
17/11/03 06:56:30 INFO security.TokenCache: Got dt for hdfs://ip-172-31-39-17.eu-central-1.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.39.17:8020, Ident: (token for frankola: HDFS_DELEGATION_TOKEN owner=frankola@SMARRONE.FNG, renewer=yarn, realUser=, issueDate=1509706590224, maxDate=1510311390224, sequenceNumber=2, masterKeyId=2)
17/11/03 06:56:30 INFO input.FileInputFormat: Total input paths to process : 50
17/11/03 06:56:30 INFO mapreduce.JobSubmitter: number of splits:50
17/11/03 06:56:30 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1509705436429_0002
17/11/03 06:56:30 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.39.17:8020, Ident: (token for frankola: HDFS_DELEGATION_TOKEN owner=frankola@SMARRONE.FNG, renewer=yarn, realUser=, issueDate=1509706590224, maxDate=1510311390224, sequenceNumber=2, masterKeyId=2)
17/11/03 06:56:31 INFO impl.YarnClientImpl: Submitted application application_1509705436429_0002
17/11/03 06:56:31 INFO mapreduce.Job: The url to track the job: http://ip-172-31-39-184.eu-central-1.compute.internal:8088/proxy/application_1509705436429_0002/
17/11/03 06:56:31 INFO mapreduce.Job: Running job: job_1509705436429_0002
17/11/03 06:56:39 INFO mapreduce.Job: Job job_1509705436429_0002 running in uber mode : false
17/11/03 06:56:39 INFO mapreduce.Job:  map 0% reduce 0%
17/11/03 06:56:46 INFO mapreduce.Job:  map 2% reduce 0%
17/11/03 06:56:47 INFO mapreduce.Job:  map 4% reduce 0%
17/11/03 06:56:49 INFO mapreduce.Job:  map 12% reduce 0%
17/11/03 06:56:51 INFO mapreduce.Job:  map 16% reduce 0%
17/11/03 06:56:55 INFO mapreduce.Job:  map 28% reduce 0%
17/11/03 06:56:59 INFO mapreduce.Job:  map 32% reduce 0%
17/11/03 06:57:01 INFO mapreduce.Job:  map 40% reduce 0%
17/11/03 06:57:03 INFO mapreduce.Job:  map 44% reduce 0%
17/11/03 06:57:07 INFO mapreduce.Job:  map 54% reduce 0%
17/11/03 06:57:08 INFO mapreduce.Job:  map 56% reduce 0%
17/11/03 06:57:11 INFO mapreduce.Job:  map 60% reduce 0%
17/11/03 06:57:14 INFO mapreduce.Job:  map 68% reduce 0%
17/11/03 06:57:15 INFO mapreduce.Job:  map 72% reduce 0%
17/11/03 06:57:19 INFO mapreduce.Job:  map 80% reduce 0%
17/11/03 06:57:20 INFO mapreduce.Job:  map 84% reduce 0%
17/11/03 06:57:23 INFO mapreduce.Job:  map 86% reduce 0%
17/11/03 06:57:24 INFO mapreduce.Job:  map 88% reduce 0%
17/11/03 06:57:25 INFO mapreduce.Job:  map 90% reduce 0%
17/11/03 06:57:26 INFO mapreduce.Job:  map 96% reduce 0%
17/11/03 06:57:27 INFO mapreduce.Job:  map 98% reduce 0%
17/11/03 06:57:30 INFO mapreduce.Job:  map 100% reduce 0%
17/11/03 06:57:31 INFO mapreduce.Job:  map 100% reduce 100%
17/11/03 06:57:31 INFO mapreduce.Job: Job job_1509705436429_0002 completed successfully
17/11/03 06:57:31 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=260
                FILE: Number of bytes written=6323599
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=15240
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=203
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=50
                Launched reduce tasks=1
                Data-local map tasks=50
                Total time spent by all maps in occupied slots (ms)=227012
                Total time spent by all reduces in occupied slots (ms)=6470
                Total time spent by all map tasks (ms)=227012
                Total time spent by all reduce tasks (ms)=6470
                Total vcore-seconds taken by all map tasks=227012
                Total vcore-seconds taken by all reduce tasks=6470
                Total megabyte-seconds taken by all map tasks=232460288
                Total megabyte-seconds taken by all reduce tasks=6625280
        Map-Reduce Framework
                Map input records=50
                Map output records=100
                Map output bytes=900
                Map output materialized bytes=1700
                Input split bytes=9340
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=1700
                Reduce input records=100
                Reduce output records=0
                Spilled Records=200
                Shuffled Maps =50
                Failed Shuffles=0
                Merged Map outputs=50
                GC time elapsed (ms)=1397
                CPU time spent (ms)=28670
                Physical memory (bytes) snapshot=22577971200
                Virtual memory (bytes) snapshot=80846667776
                Total committed heap usage (bytes)=25578438656
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=5900
        File Output Format Counters
                Bytes Written=97
Job Finished in 61.769 seconds
Estimated value of Pi is 3.14160000000000000000
```
