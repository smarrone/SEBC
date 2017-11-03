[reilly@ip-172-31-39-17 ~]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/reilly/tgen /user/reilly/tsort
17/11/03 06:49:23 INFO terasort.TeraSort: starting
17/11/03 06:49:24 INFO hdfs.DFSClient: Created token for reilly: HDFS_DELEGATION_TOKEN owner=reilly@SMARRONE.FNG, renewer=yarn, realUser=, issueDate=1509706164927, maxDate=1510310964927, sequenceNumber=1, masterKeyId=2 on 172.31.39.17:8020
17/11/03 06:49:24 INFO security.TokenCache: Got dt for hdfs://ip-172-31-39-17.eu-central-1.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.39.17:8020, Ident: (token for reilly: HDFS_DELEGATION_TOKEN owner=reilly@SMARRONE.FNG, renewer=yarn, realUser=, issueDate=1509706164927, maxDate=1510310964927, sequenceNumber=1, masterKeyId=2)
17/11/03 06:49:25 INFO input.FileInputFormat: Total input paths to process : 12
Spent 435ms computing base-splits.
Spent 5ms computing TeraScheduler splits.
Computing input splits took 441ms
Sampling 10 splits of 204
Making 10 from 100000 sampled records
Computing parititions took 821ms
Spent 1264ms computing partitions.
17/11/03 06:49:26 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-39-184.eu-central-1.compute.internal/172.31.39.184:8032
17/11/03 06:49:26 INFO mapreduce.JobSubmitter: number of splits:204
17/11/03 06:49:26 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1509705436429_0001
17/11/03 06:49:26 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.39.17:8020, Ident: (token for reilly: HDFS_DELEGATION_TOKEN owner=reilly@SMARRONE.FNG, renewer=yarn, realUser=, issueDate=1509706164927, maxDate=1510310964927, sequenceNumber=1, masterKeyId=2)
17/11/03 06:49:27 INFO impl.YarnClientImpl: Submitted application application_1509705436429_0001
17/11/03 06:49:27 INFO mapreduce.Job: The url to track the job: http://ip-172-31-39-184.eu-central-1.compute.internal:8088/proxy/application_1509705436429_0001/
17/11/03 06:49:27 INFO mapreduce.Job: Running job: job_1509705436429_0001
17/11/03 06:49:36 INFO mapreduce.Job: Job job_1509705436429_0001 running in uber mode : false
17/11/03 06:49:36 INFO mapreduce.Job:  map 0% reduce 0%
17/11/03 06:49:47 INFO mapreduce.Job:  map 1% reduce 0%
17/11/03 06:49:50 INFO mapreduce.Job:  map 3% reduce 0%
17/11/03 06:49:53 INFO mapreduce.Job:  map 4% reduce 0%
17/11/03 06:49:57 INFO mapreduce.Job:  map 5% reduce 0%
17/11/03 06:49:58 INFO mapreduce.Job:  map 6% reduce 0%
17/11/03 06:49:59 INFO mapreduce.Job:  map 7% reduce 0%
17/11/03 06:50:04 INFO mapreduce.Job:  map 8% reduce 0%
17/11/03 06:50:05 INFO mapreduce.Job:  map 10% reduce 0%
17/11/03 06:50:11 INFO mapreduce.Job:  map 12% reduce 0%
17/11/03 06:50:12 INFO mapreduce.Job:  map 13% reduce 0%
17/11/03 06:50:17 INFO mapreduce.Job:  map 14% reduce 0%
17/11/03 06:50:19 INFO mapreduce.Job:  map 15% reduce 0%
17/11/03 06:50:20 INFO mapreduce.Job:  map 16% reduce 0%
17/11/03 06:50:23 INFO mapreduce.Job:  map 17% reduce 0%
17/11/03 06:50:26 INFO mapreduce.Job:  map 18% reduce 0%
17/11/03 06:50:27 INFO mapreduce.Job:  map 19% reduce 0%
17/11/03 06:50:29 INFO mapreduce.Job:  map 20% reduce 0%
17/11/03 06:50:33 INFO mapreduce.Job:  map 21% reduce 0%
17/11/03 06:50:34 INFO mapreduce.Job:  map 22% reduce 0%
17/11/03 06:50:35 INFO mapreduce.Job:  map 23% reduce 0%
17/11/03 06:50:40 INFO mapreduce.Job:  map 24% reduce 0%
17/11/03 06:50:41 INFO mapreduce.Job:  map 25% reduce 0%
17/11/03 06:50:47 INFO mapreduce.Job:  map 26% reduce 0%
17/11/03 06:50:48 INFO mapreduce.Job:  map 28% reduce 0%
17/11/03 06:50:53 INFO mapreduce.Job:  map 29% reduce 0%
17/11/03 06:50:55 INFO mapreduce.Job:  map 30% reduce 0%
17/11/03 06:50:56 INFO mapreduce.Job:  map 31% reduce 0%
17/11/03 06:50:59 INFO mapreduce.Job:  map 32% reduce 0%
17/11/03 06:51:02 INFO mapreduce.Job:  map 33% reduce 0%
17/11/03 06:51:04 INFO mapreduce.Job:  map 34% reduce 0%
17/11/03 06:51:05 INFO mapreduce.Job:  map 35% reduce 0%
17/11/03 06:51:09 INFO mapreduce.Job:  map 36% reduce 0%
17/11/03 06:51:11 INFO mapreduce.Job:  map 37% reduce 0%
17/11/03 06:51:12 INFO mapreduce.Job:  map 38% reduce 0%
17/11/03 06:51:17 INFO mapreduce.Job:  map 39% reduce 0%
17/11/03 06:51:18 INFO mapreduce.Job:  map 40% reduce 0%
17/11/03 06:51:20 INFO mapreduce.Job:  map 41% reduce 0%
17/11/03 06:51:23 INFO mapreduce.Job:  map 42% reduce 0%
17/11/03 06:51:24 INFO mapreduce.Job:  map 43% reduce 0%
17/11/03 06:51:27 INFO mapreduce.Job:  map 44% reduce 0%
17/11/03 06:51:29 INFO mapreduce.Job:  map 45% reduce 0%
17/11/03 06:51:31 INFO mapreduce.Job:  map 46% reduce 0%
17/11/03 06:51:34 INFO mapreduce.Job:  map 47% reduce 0%
17/11/03 06:51:35 INFO mapreduce.Job:  map 48% reduce 0%
17/11/03 06:51:40 INFO mapreduce.Job:  map 49% reduce 0%
17/11/03 06:51:41 INFO mapreduce.Job:  map 50% reduce 0%
17/11/03 06:51:43 INFO mapreduce.Job:  map 51% reduce 0%
17/11/03 06:51:48 INFO mapreduce.Job:  map 53% reduce 0%
17/11/03 06:51:50 INFO mapreduce.Job:  map 54% reduce 0%
17/11/03 06:51:55 INFO mapreduce.Job:  map 55% reduce 0%
17/11/03 06:51:56 INFO mapreduce.Job:  map 56% reduce 0%
17/11/03 06:51:57 INFO mapreduce.Job:  map 57% reduce 0%
17/11/03 06:52:01 INFO mapreduce.Job:  map 58% reduce 0%
17/11/03 06:52:04 INFO mapreduce.Job:  map 60% reduce 0%
17/11/03 06:52:07 INFO mapreduce.Job:  map 61% reduce 0%
17/11/03 06:52:11 INFO mapreduce.Job:  map 62% reduce 0%
17/11/03 06:52:12 INFO mapreduce.Job:  map 63% reduce 0%
17/11/03 06:52:13 INFO mapreduce.Job:  map 64% reduce 0%
17/11/03 06:52:17 INFO mapreduce.Job:  map 65% reduce 0%
17/11/03 06:52:19 INFO mapreduce.Job:  map 66% reduce 0%
17/11/03 06:52:20 INFO mapreduce.Job:  map 67% reduce 0%
17/11/03 06:52:25 INFO mapreduce.Job:  map 69% reduce 0%
17/11/03 06:52:28 INFO mapreduce.Job:  map 70% reduce 0%
17/11/03 06:52:32 INFO mapreduce.Job:  map 71% reduce 0%
17/11/03 06:52:33 INFO mapreduce.Job:  map 72% reduce 0%
17/11/03 06:52:37 INFO mapreduce.Job:  map 73% reduce 0%
17/11/03 06:52:38 INFO mapreduce.Job:  map 74% reduce 0%
17/11/03 06:52:40 INFO mapreduce.Job:  map 75% reduce 0%
17/11/03 06:52:45 INFO mapreduce.Job:  map 76% reduce 0%
17/11/03 06:52:47 INFO mapreduce.Job:  map 77% reduce 0%
17/11/03 06:52:48 INFO mapreduce.Job:  map 78% reduce 0%
17/11/03 06:52:52 INFO mapreduce.Job:  map 79% reduce 0%
17/11/03 06:52:54 INFO mapreduce.Job:  map 80% reduce 0%
17/11/03 06:52:55 INFO mapreduce.Job:  map 81% reduce 0%
17/11/03 06:52:59 INFO mapreduce.Job:  map 82% reduce 0%
17/11/03 06:53:01 INFO mapreduce.Job:  map 83% reduce 0%
17/11/03 06:53:03 INFO mapreduce.Job:  map 84% reduce 0%
17/11/03 06:53:06 INFO mapreduce.Job:  map 85% reduce 0%
17/11/03 06:53:11 INFO mapreduce.Job:  map 85% reduce 3%
17/11/03 06:53:12 INFO mapreduce.Job:  map 86% reduce 3%
17/11/03 06:53:13 INFO mapreduce.Job:  map 86% reduce 6%
17/11/03 06:53:15 INFO mapreduce.Job:  map 86% reduce 11%
17/11/03 06:53:18 INFO mapreduce.Job:  map 87% reduce 12%
17/11/03 06:53:24 INFO mapreduce.Job:  map 88% reduce 12%
17/11/03 06:53:30 INFO mapreduce.Job:  map 89% reduce 12%
17/11/03 06:53:36 INFO mapreduce.Job:  map 90% reduce 12%
17/11/03 06:53:42 INFO mapreduce.Job:  map 91% reduce 12%
17/11/03 06:53:47 INFO mapreduce.Job:  map 92% reduce 12%
17/11/03 06:53:52 INFO mapreduce.Job:  map 93% reduce 12%
17/11/03 06:53:57 INFO mapreduce.Job:  map 94% reduce 12%
17/11/03 06:54:02 INFO mapreduce.Job:  map 95% reduce 12%
17/11/03 06:54:03 INFO mapreduce.Job:  map 95% reduce 13%
17/11/03 06:54:07 INFO mapreduce.Job:  map 96% reduce 13%
17/11/03 06:54:13 INFO mapreduce.Job:  map 97% reduce 13%
17/11/03 06:54:19 INFO mapreduce.Job:  map 98% reduce 13%
17/11/03 06:54:25 INFO mapreduce.Job:  map 99% reduce 13%
17/11/03 06:54:30 INFO mapreduce.Job:  map 100% reduce 13%
17/11/03 06:54:37 INFO mapreduce.Job:  map 100% reduce 17%
17/11/03 06:54:38 INFO mapreduce.Job:  map 100% reduce 13%
17/11/03 06:54:45 INFO mapreduce.Job:  map 100% reduce 16%
17/11/03 06:54:46 INFO mapreduce.Job:  map 100% reduce 21%
17/11/03 06:54:48 INFO mapreduce.Job:  map 100% reduce 25%
17/11/03 06:54:49 INFO mapreduce.Job:  map 100% reduce 28%
17/11/03 06:54:50 INFO mapreduce.Job:  map 100% reduce 32%
17/11/03 06:54:51 INFO mapreduce.Job:  map 100% reduce 34%
17/11/03 06:54:52 INFO mapreduce.Job:  map 100% reduce 37%
17/11/03 06:54:53 INFO mapreduce.Job:  map 100% reduce 42%
17/11/03 06:54:54 INFO mapreduce.Job:  map 100% reduce 44%
17/11/03 06:54:55 INFO mapreduce.Job:  map 100% reduce 46%
17/11/03 06:54:56 INFO mapreduce.Job:  map 100% reduce 52%
17/11/03 06:54:57 INFO mapreduce.Job:  map 100% reduce 53%
17/11/03 06:54:58 INFO mapreduce.Job:  map 100% reduce 54%
17/11/03 06:54:59 INFO mapreduce.Job:  map 100% reduce 57%
17/11/03 06:55:02 INFO mapreduce.Job:  map 100% reduce 58%
17/11/03 06:55:05 INFO mapreduce.Job:  map 100% reduce 63%
17/11/03 06:55:07 INFO mapreduce.Job:  map 100% reduce 67%
17/11/03 06:55:08 INFO mapreduce.Job:  map 100% reduce 74%
17/11/03 06:55:09 INFO mapreduce.Job:  map 100% reduce 78%
17/11/03 06:55:10 INFO mapreduce.Job:  map 100% reduce 81%
17/11/03 06:55:11 INFO mapreduce.Job:  map 100% reduce 85%
17/11/03 06:55:12 INFO mapreduce.Job:  map 100% reduce 88%
17/11/03 06:55:14 INFO mapreduce.Job:  map 100% reduce 90%
17/11/03 06:55:15 INFO mapreduce.Job:  map 100% reduce 92%
17/11/03 06:55:16 INFO mapreduce.Job:  map 100% reduce 93%
17/11/03 06:55:17 INFO mapreduce.Job:  map 100% reduce 95%
17/11/03 06:55:18 INFO mapreduce.Job:  map 100% reduce 96%
17/11/03 06:55:19 INFO mapreduce.Job:  map 100% reduce 98%
17/11/03 06:55:20 INFO mapreduce.Job:  map 100% reduce 99%
17/11/03 06:55:21 INFO mapreduce.Job:  map 100% reduce 100%
17/11/03 06:55:22 INFO mapreduce.Job: Job job_1509705436429_0001 completed successfully
17/11/03 06:55:23 INFO mapreduce.Job: Counters: 51
        File System Counters
                FILE: Number of bytes read=2910007340
                FILE: Number of bytes written=5782893157
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=6553631008
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=642
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=20
        Job Counters
                Killed reduce tasks=2
                Launched map tasks=204
                Launched reduce tasks=12
                Data-local map tasks=198
                Rack-local map tasks=6
                Total time spent by all maps in occupied slots (ms)=1172484
                Total time spent by all reduces in occupied slots (ms)=599112
                Total time spent by all map tasks (ms)=1172484
                Total time spent by all reduce tasks (ms)=599112
                Total vcore-seconds taken by all map tasks=1172484
                Total vcore-seconds taken by all reduce tasks=599112
                Total megabyte-seconds taken by all map tasks=1200623616
                Total megabyte-seconds taken by all reduce tasks=613490688
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Map output bytes=6684672000
                Map output materialized bytes=2846186245
                Input split bytes=31008
                Combine input records=0
                Combine output records=0
                Reduce input groups=65536000
                Reduce shuffle bytes=2846186245
                Reduce input records=65536000
                Reduce output records=65536000
                Spilled Records=131072000
                Shuffled Maps =2040
                Failed Shuffles=0
                Merged Map outputs=2040
                GC time elapsed (ms)=15637
                CPU time spent (ms)=888210
                Physical memory (bytes) snapshot=103933988864
                Virtual memory (bytes) snapshot=339110871040
                Total committed heap usage (bytes)=121167675392
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
17/11/03 06:55:23 INFO terasort.TeraSort: done
