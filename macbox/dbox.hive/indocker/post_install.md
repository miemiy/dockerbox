

###
Install git from IUS
```
sudo yum -y install  git2u-all
#####

## jdk installation

http://webfile.bluesky.lab.home:10080/appbox/jdk/jdk-8u131-linux-x64.tar.gz



[admin@hive appbox]$ pwd
/ext/appbox

$ curl -O http://webfile.bluesky.lab.home:10080/appbox/jdk/jdk-8u131-linux-x64.tar.gz

tar zxvf jdk-8u131-linux-x64.tar.gz


####
[admin@hive ~]$ pwd
/home/admin
[admin@hive ~]$ mkdir bin
[admin@hive ~]$ ls
bin
[admin@hive ~]$ cd bin
[admin@hive bin]$ ls
[admin@hive bin]$ pwd
/home/admin/bin
[admin@hive bin]$

$ curl -O http://webfile.bluesky.lab.home:10080/bigdata/apache-hive-2.3.5-bin.tar.gz
$ curl -O http://webfile.bluesky.lab.home:10080/bigdata/hadoop-2.9.2.tar.gz



[admin@hive bigdata]$ pwd
/ext/bigdata
[admin@hive bigdata]$ ls -l
total 12
drwxrwxr-x 3 admin admin 4096 Oct 27 15:30 hadoop
drwxrwxr-x 2 admin admin 4096 Oct 27 15:30 hive
drwxrwxr-x 2 admin admin 4096 Oct 27 15:26 packages
[admin@hive bigdata]$
[admin@hive hadoop]$ pwd
/ext/bigdata/hadoop
[admin@hive hadoop]$
[admin@hive hadoop]$ tar zxvf ../packages/hadoop-2.9.2.tar.gz

[admin@hive hadoop]$ cd ..
[admin@hive bigdata]$ ls
hadoop  hive  packages
[admin@hive bigdata]$ cd hive
[admin@hive hive]$ ls
[admin@hive hive]$ pwd
/ext/bigdata/hive
[admin@hive hive]$ 
[admin@hive hive]$ tar zxvf ../packages apache-hive-2.3.5-bin.tar.gz
