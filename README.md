##Auth over ssh

You can use ssh port forwarding to encrypt the protocol. To forward
the remote system's port 564 to localhosts's port 9999:

```
  ssh -L 9999:localhost:564 user@server &
```
##Mmount
```
9pfuse 'tcp!127.0.0.1!9999'  /home/komar/mnt/
```

##Unmount
```
fusermount -u -z /home/komar/mnt/
```