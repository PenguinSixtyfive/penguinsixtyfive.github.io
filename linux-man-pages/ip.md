# IP

Show & manipulate routing, network devices, interfaces and tunnels.

### Common Objects 

| Option | Description |
| --- | --- |
| address | Protocol (IP or IPv6) address on a device |
| addrlabel | Label configuration for protocol address selection |
| l2tp | tunnel ethernet over IP (L2TPv3) |
| link | Network device |
| monitor | Watch for netlink messages |
| neighbour | Manage ARP or NDISC cache entries |
| netns | Manage network namespaces |
| route  | Routing table entry |
| stats | Manage and show interface statistics |
| tcpmetrics | Manage TCP Metrics |
| tunnel | Tunnel over IP |

### Common Options

| Option | Description |
| --- | --- |
| -b `FILE ` | Read commands from provided file or standard input and invoke them |
| -br | Print only basic information in a tabular format for better readability |
| -h | Output statistics with human readable values |
| -j | Output results in JSON format |
| -l | Specify maximum number of loops the `ip address flush` logic will attempt before giving up. Default is 10. Zero `0` means loop until all addresses are removed |
| -o | Output each record on a single line |
| -p | With `-j` adds indentation for readability |
| -s | Output more statistics |
| -ts | Like `-t`, but use shorter format |
| -0 | Shortcut for `-family link` |
| -4 | Shortcut for `-family inet` |
| -6 | Shortcut for `-family inet6` |

### Note

* The names of all objects may be written in full or abbreviated form, for example `address` can be abbreviated as `addr` or just `a`.

### [Back](linux-man-pages.md)
