# dockerbox

docker box for nannar lab

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


