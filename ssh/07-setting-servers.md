# Set up

To install an SSH server software on Debian:

```bash
sudo apt install openssh-server
```

Then, start or enable the service:

```bash
systemctl enable sshd.service
```

Common configs in `/etc/ssh/sshd_config`:

* #Port 22                        uncomment to change the listening port
* #LoginGraceTime 2m
* #PermitRootLogin Yes            uncomment to change to no so you can't login as root
* #PasswordAuthentication         disable user password logins, and use keys only
* #Banner <path to file.txt>      display a messge when user logs in

You will have to reboot the server for these changes to take effect.


