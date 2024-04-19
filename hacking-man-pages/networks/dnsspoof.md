# DNSSPOOF

Forge replies to DNS address & pointer queries.

### Common Options

| Option | Desciption |
| --- | --- |
| -i `interface` | Specify the interface to use |
| -f `hosts-file` | Specify the file in `hosts` format. No aliases, although host-names may contain wildcards |
| `expression` | Specify a `tcpdump` filter expression to select traffic to sniff |

### Files

* `/usr/share/dsniff/dnsspoof.hosts`: Sample hosts file.

### Notes

* If no `hostsfile` is specified, replies will be forged for all address queries on the LAN with an answer of the local machine's IP address.



