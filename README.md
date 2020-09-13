# dockerbox

docker box for nannar lab

## Purpose

### 1. Bluesky  
Bluesky box can be hosted in nannar server and as service to whole lab. 
Such as GitLab(github),gitea (github) Seafile (could file), Nginx(Web file server), bind(dns)

### 2. SrvBox
SrvBox is docker as service in the local machine and can be inter-communicate with other app such IDE. The most important thing is the service should be like a natived installed server which can handle local resources instead of docker inside only.

For example, a nginx(proxy) which can proxy a spring boot service running inside IDE. 

### 3. DevEnv Box
DevEnv box can be a cluster of docker containers which inter-communicate each other only. That means those container themselves are virtually in a LAN area. Except some special web port and shared local directory, they do not need commuicate with app in the host machine. 


## Convention


### dir prefix
bluesky  for service


dbox obsolete , replaced by devenv 


devenv for setting dev environment in local machine


### dir post fix

<default>   for linux host

.win for windows host, becasue  mount directory will be different.  On windows, using git-bash


### source file location

bluesky.nginx 
dns:  gitlab.lab.home  port: 10080
-  change in linux and mac : in /etc/hosts
-  change in windows: C:\Windows\System32\drivers\etc\hosts

```
<local_ip_dhcp> gitlab.lab.home

```

## Port Range for internal using

 - devenv.centos.ssh:  Internal Index 2 -   port 102xx
 - devenv.centos.vue.win: Internal Index 3 -   port 103xx


@end


