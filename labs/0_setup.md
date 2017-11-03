Cloude Provider: AWS

IP address and DNS name:
54.93.230.44	ec2-54-93-230-44.eu-central-1.compute.amazonaws.com
18.194.45.138	ec2-18-194-45-138.eu-central-1.compute.amazonaws.com
54.93.56.242	ec2-54-93-56-242.eu-central-1.compute.amazonaws.com
52.59.210.215	ec2-52-59-210-215.eu-central-1.compute.amazonaws.com
54.93.226.7	ec2-54-93-226-7.eu-central-1.compute.amazonaws.com

Linux release:
uname -a
Linux ip-172-31-44-186.eu-central-1.compute.internal 3.10.0-327.36.3.el7.x86_64 #1 SMP Thu Oct 20 04:56:07 EDT 2016 x86_64 x86_64 x86_64 GNU/Linux

File system capacity for the first node:
df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       50G  933M   50G   2% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   17M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000


yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
rhui-REGION-client-config-server-7                                                                                                               | 2.9 kB  00:00:00
rhui-REGION-rhel-server-releases                                                                                                                 | 3.5 kB  00:00:00
rhui-REGION-rhel-server-rh-common                                                                                                                | 3.8 kB  00:00:00
(1/7): rhui-REGION-rhel-server-releases/7Server/x86_64/group                                                                                     | 709 kB  00:00:00
(2/7): rhui-REGION-client-config-server-7/x86_64/primary_db                                                                                      | 4.9 kB  00:00:00
(3/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/group                                                                                    |  104 B  00:00:00
(4/7): rhui-REGION-rhel-server-releases/7Server/x86_64/updateinfo                                                                                | 2.4 MB  00:00:00
(5/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/updateinfo                                                                               |  32 kB  00:00:00
(6/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/primary_db                                                                               | 119 kB  00:00:00
(7/7): rhui-REGION-rhel-server-releases/7Server/x86_64/primary_db                                                                                |  44 MB  00:00:00
repo id                                                                  repo name                                                                                status
rhui-REGION-client-config-server-7/x86_64                                Red Hat Update Infrastructure 2.0 Client Configuration Server 7                               5
rhui-REGION-rhel-server-releases/7Server/x86_64                          Red Hat Enterprise Linux Server 7 (RPMs)                                                 17,471
rhui-REGION-rhel-server-rh-common/7Server/x86_64                         Red Hat Enterprise Linux Server 7 RH Common (RPMs)                                          228
repolist: 17,704

