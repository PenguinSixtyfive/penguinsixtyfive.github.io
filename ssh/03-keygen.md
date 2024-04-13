# Generating keys

Connecting using a key pair is more secure than a username and password.

The key pair are:
1. Public key
You can share this key with servers and other users.
2. Private key
This is **not** to be shared under any circumstances.

You can generate multiple private keys to connect from different computers, or copy the same private key over.
Generating multiple keys requires a bit more setup, but is considered a safer option.

To generate a key:
```bash
ssh-keygen -t rsa
```

Follow the interactive prompts
The `passphrase` is to unlock the key, not a user password.
The random art image is used to verify the key, but most likely won't be used.

To copy the public key to a server:
```bash
ssh-copy-id <user>@<server>
```
or:
```bash
scp <key.pub> <user>@<server>
```

After connecting to the server, `cat` the key to the `authorized_keys` file:

```bash
cat <key.pub> >> .ssh/authorized_keys
```

After copying the pub key to the server, you can connect to the server using the private key:

```bash
ssh -i .ssh/<key> <user>@<server>
```


