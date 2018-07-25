## Mount
```
9pfuse 'tcp!127.0.0.1!9999'  ~/mnt/
```

## Unmount
```
fusermount -u -z ~/mnt/
```

## Auth over ssh

You can use ssh port forwarding to encrypt the protocol. To forward
the remote system's port 564 to localhosts's port 9999:

```
  ssh -L 9999:localhost:9999 user@server 
```
