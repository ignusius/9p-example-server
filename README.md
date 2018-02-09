#Auth over ssh

You can use ssh port forwarding to encrypt the protocol. To forward
the remote system's port 564 to localhosts's port 9999:

```
  ssh -L 9999:localhost:564 user@server &
```