# WAFW00F

Identify and fingerprint Web Application Firewall products.

### Common Options

| Option | Description |
| --- | --- |
| -a | Find all WAFs, do not stop testing on the first one |
| -r | Do not follow redirections given by 3xx responses |
| -t `waf` | Test for one specific WAF product |
| -o `file` | Write output to csv, json or text file depending on file extension |
| -i `file` | Read targets from a file. For csv and json, a `url` column name or element is required |
| -l | List all the WAFs that `wafw00f` is able to detect |
| -p `proxy` | Use an HTTP proxy to perform requests, example: http://hostname:8080, socks5://hostname:1080 |
| -H `file` | Pass custom headers, for example to overwrite the default user-agent string |



