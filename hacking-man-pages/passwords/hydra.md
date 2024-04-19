# HYDRA

A parallelized network login cracker, supporting numerous protocols to attack.

* `target`: A target to attack, can be an IPv4 address, IPv6 address or DNS name.
* `service`: A service to attack, see the list of protocols available.

### Common Options

| Option | Description |
| --- | --- |
| -b `format` | Specify the format for the `-o file`: text, json, jsonv1 |
| -c `time` | The wait time in seconds per login attempt over all threads |
| -C `file` | Colon separated `login:pass` format, instead of `-L` and `-P` options |
| -e `nsr` | Additional checks, `n` for null password, `s` try login as pass, `r` try the reverse login as pass |
| -f | Exit after the first found login/password pair (per host if -M) |
| -F | Exit after the first found login/password pair for any host (for usage with -M) |
| -I | Ignore an existing restore file (don't wait 10 seconds) |
| -l `login` | Login with the given username |
| -L `file` | Load sever logins from `file` |
| -m `options` | Module specific options. See hydra `-U module` for  available options |
| -M `file` | Server list for parallel attacks, one entry per line |
| -o `file` | Write found login/password pairs to `file` instead of `stdout` |
| -O | Use old SSL v2 and v3 |
| -p `pass` | Try given password |
| -P `file` | Try several passwords from `file` |
| -R | Restore a previously aborted session. Requires a `hydra.restore` file |
| -s `port` | If the service is on a different default port, define it here |
| -S | Connect via SSL |
| -t `tasks` | Run `tasks` number of connects in parallel (default = 16) |
| -u | Loop around the passwords in a list, so the first password is tried on all logins, then the next password |
| -U `servicename` | Get help on the optional or mandatory options of a service |
| -w `time` | Defines the max wait time in seconds for responses (default = 32) |
| -W `time` | Defines a wait time between each connection a task performs |
| -x `min:max:charset` | Generate passwords from `min` to `max` length, `1` for numbers, `a,A` for letters |
| -y | Disable use of symbols in `-x` brute-force |
| -4 , -6 | Prefer IPv4 (default) or IPv6 addresses |

### Supported Services

| | | | | |
| --- | --- | --- | --- | --- | 
| adam6500 | afp | asterisk | cisco | cisco-enable |
| cvs | firebird | ftp | ftps | http(s)-{head,get,post} |
| http(s)-{get,post}-form | http-proxy | http-proxy-urlenum | icq | imap(s) |
| irc | ldap2(s) | ldap3-{cram,di‐gest}md5(s) | mssql | mysql(v4) |
| mysql5 | ncp | nntp | oracle | oracle-listener |
| oracle-sid | pcanywhere | pcnfs | pop3(s) | postgres |
| rdp | radmin2 | redis | rexec | rlogin |
| rpcap | rsh | rtsp | s7-300 | sapr3 |
| sip | smb | smtp(s) | smtp-enum snmp | socks5 |
| ssh | sshkey | svn | teamspeak | telnet(s) |
| vmauthd | vnc | xmpp |


