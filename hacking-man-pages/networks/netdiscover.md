# NETDISCOVER

Active/passive ARP reconnaissance tool.

### Common Options

| Option | Description |
| --- | --- |
| -c `count` | Number of times to send each ARP request (default = 1) |
| -d | Ignore configuration files at `home dir` (for autoscan and fast mode only) |
| -f | Fast mode scan. Only scan for .1, .100 and .254 on each network |
| -F `filter` | Customize `pcap` filter expression (default = arp) |
| -i `device` | The network interface to sniff and inject packets |
| -l `file` | Scan ranges from `file`. Must be one range per line |
| -L | Similar to `-P` but continue program execution to capture ARP packets passively after the active scan |
| -m `file` | Scan a list of known `MACs` and host names |
| -n `node` | Last IP octet of the source IP used for scanning (allowed range = 2-253, default = 67) |
| -N | Do not print header. Only valid when `-P` or `-L` is enabled |
| -p | Passive mode. `netdiscover` does not send anything, but does only sniff |
| -P | Produces an output suitable to be redirected into a file or to be parsed by another program |
| -r `range` | Scan a given range instead of auto scan |
| -s `time` | Sleep given time in milliseconds between each ARP request injection (default = 1) |

### Notes

* `netdiscover` will look for 2 config files each time it is executed. If they don't exist, it will use default values.
* For examples and use-cases, refer to the manual.


