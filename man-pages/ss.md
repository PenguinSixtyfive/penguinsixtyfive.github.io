# SS

Another utility to investigate & dump socket statistics.\
It allows showing information similar to `netstat`.\
It can display more TCP and state information than other tools.

### Common Options

| Option | Description |
| --- | --- |
| -a | Display both listening and non-listening sockets |
| -D `FILE` | Do not display anything, just dump raw information about TCP sockets to `FILE` after applying filters |
| -e | Show detailed socket information. Refer to the manual for output format |
| -E | Continually display sockets as they are destroyed |
| -F FILE | Read filter information from `FILE` |
| -H | Suppress header line |
| -K | Attempts to forcibly close (kill) sockets. It supports IPv4 and IPv6 sockets only |
| -l | Display only listening sockets |
| -O | Print each socket's data on a single line |
| -p | Show process using socket |
| -r | Try to resolve numeric address/ports |
| -s | Print summary statistics |
| -t | Display TCP sockets |
| -u | Display UDP sockets |
| -w | Display RAW sockets |
| -x | Display Unix domain sockets |
| -z | Like `-Z` option but also shows the socket context |
| -Z | Like`-p` option but also shows process security context. If `-T` is used, also shows thread security context |
| -0 | Display `PACKET` sockets |
| -4 | Display only IPv4 sockets |
| -6 | Display only IPv6 sockets |

### Note
When no option is used, `ss` displays a list of open non-listening sockets that have established connection.



