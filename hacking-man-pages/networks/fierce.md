# FIERCE

DNS scanner that helps locate non-contiguous IP space and hostnames against specified domains.

### Common Options

| Option | Description |
| --- | --- |
| --connect | Attempt an HTTP connection to non-RFC 1918 hosts |
| --delay `delay` | Time to wait between lookups |
| --domain `domain` | Domain name to test |
| --dns-file `file` | Use DNS servers specified in this file for reverse lookups (one per line) |
| --dns-servers `server` | Use these DNS servers for reverse lookups, separated by commas |
| --range `range` | Scan an internal IP range, use `cidr` notation |
| --search `search` | Filter on these domains when expanding lookup, separate searches by commas |
| --subdomains `subdomains` | Use these subdomains, separated by commas |
| --subdomain-file `file` | Use the subdomains specified in this file (one per line) |
| --traverse `traverse` | Scan IPs near discovered records, this won't enter adjacent class C's |
| --tcp | Use TCP instead of UDP |
| --wide | Scan entire class c of discovered records |

* For examples, refer to the manual.



