# Connecting to a server

To connect to an SSH server:

```bash
ssh <user>@<server>
```

When connecting to a server for the first time, you will be prompted to accept the server key.  
The key will be stored in `$HOME/.ssh/known_hosts` on the server and local machine.  
If a server you connected to before prompts you for the key again, investigate before accepting the new key.

If the server is not running on port 22:

```bash
ssh -p# <user>@<server>
```


