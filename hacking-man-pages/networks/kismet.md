# KISMET

Wireless sniffer and monitor.

### Common Options

| Option | Description |
| --- | --- |
| -f `file` | Use alternate config file |
| -s | Turn off `stdout` output after setup phase |
| --daemonize | Spawn detached in the background |
| --debug | Disable the console wrapper and the crash handling functions, for debugging |
| --homedir `path` | Use an alternate path as the home directory instead of the user entry |
| --confdir `path` | Use an alternate path as the base config directory instead of the default set at compile time |
| --datadir `path` | Use an alternate path as the data directory instead of the default set at compile time |
| --no-console-wrapper | Disable server console wrapper |
| --no-ncurses-wrapper | Disable server console wrapper |
| --no-line-wrap | Turn of line-wrapping of output (for grep, speed, etc) |
| --no-plugins | Do not load plugins |

### Logging Options

| Option | Description |
| --- | --- |
| -n | Disable logging entirely |
| -t `title` | Override default log title |
| -T `types` | Override activated log types |
| -p `prefix` | Directory to store log files |
| --device-timeout=n | Expire devices after `n` seconds |

### Notes
* Nearly all of these options are run-time overrides for values in the `kismet.conf` config file.
* Permanent changes should be made to the configuration file.


