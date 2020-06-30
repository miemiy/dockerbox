


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

