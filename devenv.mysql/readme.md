   
```bash

$ docker volume create mysqldata
mysqldata

jaco@KOTIN MINGW64 ~
$ docker volume inspect mysqldata
[
    {
        "CreatedAt": "2020-02-29T10:36:06Z",
        "Driver": "local",
        "Labels": {},
        "Mountpoint": "/var/lib/docker/volumes/mysqldata/_data",
        "Name": "mysqldata",
        "Options": {},
        "Scope": "local"
    }
]

```



```bash

create user 'jaco'@'%' identified by 'blueskypwd';
grant all privileges on *.* to 'jaco'@'%' with grant option;
```


