
# vuehack

## Available 2020-09-30

## source code 


## IDE:VSCode
In order to user vscode remote, need to expose ssh port to host machine



```
ssh -p 10322 app-admin@localhost
```
PasswordAuthentication enabled
If connecting to a container running with SSH_PASSWORD_AUTHENTICATION set to "true" the process of connecting is simplified and the command used differs slightly.

```
$ ssh \
  -o Port={{container-port}} \
  -o StrictHostKeyChecking=no \
  -o UserKnownHostsFile=/dev/null \
  app-admin@{{docker-host-ip}}

$ ssh -o Port=10322 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null admin@localhost
```

