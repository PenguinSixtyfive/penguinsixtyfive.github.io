# Copying files

`FileZilla` is A GUI app to transfer files over SSH.

At the top, enter server, user and password, and port details.
* The right pane displays the remote machine (server).
* The left pane displays the local machine.

To copy files at the terminal:

```bash
sftp <usr>@<server>
```

To exit `sftp`, type `bye`.

For quick transfers, use `Secure Copy`:

```bash
scp <file> <user>@<server>:
```

The colon at the end will copy the files to the `$HOME` directory on the server.  
You could also specify a path after the colon.

To copy files from the server to the local machine:

```bash
scp <user>@<server>:<file> <directory on local machine>
```


