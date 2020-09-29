
# SSH

## Available 2020-09-30

## connect from host using ss

$ ssh -o Port=10022 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null admin@localhost
$ sftp  -o Port=10022 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null admin@localhost

$ ssh -L 127.0.0.1:10900:nginx.dev:80 -o Port=10022 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null admin@localhost
  