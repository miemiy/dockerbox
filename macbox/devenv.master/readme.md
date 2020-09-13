
# SSH

## connect from host using ss

$ ssh -o Port=10022 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null admin@localhost
$ sftp  -o Port=10022 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null admin@localhost
  