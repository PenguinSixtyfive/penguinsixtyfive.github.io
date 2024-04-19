# DIRB

A Web Content Scanner, searching for existing or hidden web objects on a server.

### Common Options

| Option | Description |
| --- | --- |
| -a `agent` | Specify your custom `user_agent` (defaults = Mozilla 4.0, MsIE 6.0, Windows NT 5.1) |
| -b | Don't squash or merge sequences of `/../` or `/./` in the given URL |
| -c `cookie` | Set a cookie for the HTTP request |
| -E `cert` | Use the specified client certificate file |
| -f | Fine-tuning of `Not found 404` detection |
| -H `header` | Add a custom header to the HTTP request |
| -i | Use case-insensitive Search |
| -l | Print `Location` header when found |
| -N `nf_code` | Ignore responses with this HTTP code |
| -o `file` | Save output to `file` |
| -p `proxy(:port)` | Use this proxy (default port = 1080) |
| -P `proxy_user:proxy_pass` | Proxy Authentication |
| -r | Do not Search Recursively |
| -R | Interactive Recursion. Ask in which directories you want to scan |
| -S | Silent Mode. Don't show tested words |
| -t | Don't force an ending `/` on URLs |
| -u `username:password` | Username and password to use |
| -v | Also show `not existent` pages |
| -w | Don't Stop on `WARNING` messages |
| -x `extensions_file` | Amplify search with the extensions on this file |
| -X `extensions` | Amplify search with this extensions |
| -z `milisecs` | Separate search requests by milliseconds |


