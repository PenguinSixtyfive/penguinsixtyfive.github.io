# PASSWD

Change passwords for user accounts.

### Common Options

| Option | Description |
| --- | --- |
| -a | This option can be used only with -S and causes show status for all users |
| -d | Delete a user's password (make it empty) |
| -e | Immediately expire an account's password |
| -i `inactive` | Disable an account after the password has been expired for a number of days |
| -l | Lock (disable) the password of the named account |
| -n `min-days` | Set the minimum number of days between password changes to `min-days` |
| -S | Display account status information. It consists of 7 fields. Refer to the manual for more info |
| -u | Unlock the password of the named account. Re-enables a password by changing it back to its previous value (before `-l`) |
| -w | Set the number of days of warning before a password change is required |
| -x `max-days` | Set the maximum number of days a password remains valid |

### [Back](linux-man-pages.md)
