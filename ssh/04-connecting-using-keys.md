# Connecting using keys

After copying the public key to the server, you can connect to the server using the private key:

```bash
ssh -i .ssh/<key> <user>@<server>
```

An easier way to connect to a server is:\
Make a `config` file in `$HOME/.ssh/`, then in it type:
```
Host <shortcut name>
    User <username>
    HostName <server
    IdentityFile $HOME/<path to priv key>
```

To connect:
```bash
ssh <shortcut name>
```

[* Back to SSH](00-ssh.md)

