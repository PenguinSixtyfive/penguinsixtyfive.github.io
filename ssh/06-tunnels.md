# SSH Tunneling

To start a local port-forwarding connection:

```bash
ssh -L <local port>:localhost:<port at server> <usr>@<server>
```

In this context, `localhost` means the server, not the local machine.

If you don't want a full connection, use the `-N` option.




