# Set up

To install an SSH server software on Debian (or Debian-based distros):

```bash
sudo apt install openssh-server
```

Then, start or enable the service:

```bash
systemctl enable sshd.service
```

Common configs in `/etc/ssh/sshd_config`:
| Comment | Description|
| --- | --- |
| * #Port 22  | Uncomment to change the listening port |
| * #LoginGraceTime 2m | - |
| #PermitRootLogin Yes | Uncomment to change to no so you can't login as `root` |
| #PasswordAuthentication | Disable user password logins, and use keys only |
| #Banner <path to file.txt> | Display a message when user logs in |

You will have to reboot the server for these changes to take effect.

[* Back to SSH](00-ssh.md)

