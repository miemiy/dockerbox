

###
Install git from IUS
```
sudo yum -y install  git2u-all
#####

####
###for netcat in centos7
[root@flink ~]# yum install nmap


####

## jdk installation

http://webfile.bluesky.lab.home:10080/appbox/jdk/jdk-8u131-linux-x64.tar.gz



$ pwd
/ext/appbox

$ curl -O http://webfile.bluesky.lab.home:10080/appbox/jdk/jdk-8u131-linux-x64.tar.gz

tar zxvf jdk-8u131-linux-x64.tar.gz

[admin@flink packages]$ pwd
/ext/bigdata/packages
[admin@flink packages]$ curl -O http://webfile.bluesky.lab.home:10080/bigdata/flink/flink-1.9.1-bin-scala_2.12.tgz
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  234M  100  234M    0     0  36.0M      0  0:00:06  0:00:06 --:--:-- 36.3M


[admin@flink bigdata]$ pwd
/ext/bigdata
[admin@flink bigdata]$ ls
packages
[admin@flink bigdata]$

[admin@flink flink]$ pwd
/ext/bigdata/flink
[admin@flink flink]$ tar zxvf ../packages/flink-1.9.1-bin-scala_2.12.tgz

