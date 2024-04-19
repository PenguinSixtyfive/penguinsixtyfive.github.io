# AIRCRACK-NG

An `802.11 WEP` and `WPA-PSK` key cracker.

### Common Options:

| Option | Description |
| --- | --- |
| -a `amode` | Force the attack mode. `1`, `wep` = WEP (802.11) `2`, `wpa` = WPA/WPA2 PSK (802.11i and 802.11w) |
| -b `bssid` | Select the target network based on the access point MAC address |
| -C `macs` | Merges all those APs MAC (separated by a comma) into a virtual one |
| -e `essid` | Select the target network based on the `ESSID` |
| -l `file` | Write the key into a file. Overwrites the file if it already exists |
| -p `nbcpu` | Set the number of CPUs to use for cracking the key/passphrase |
| -q  | No status information is displayed |

### Static WEP cracking options:

| Option | Description |
| --- | --- |
| -c | Search alpha-numeric characters only |
| -d `mask` | Specify mask of the key. For example: `A1:XX:CF` |
| -D | WEP decloak mode |
| -f `fudge` | Use a higher value to increase the brute-force level (default = 2) |
| -h | Search the numeric key for Fritz!BOX |
| -i `index` | Only keep the IVs that have this key index (1 to 4). By default it ignores the key index, and uses the IV |
| -k `korek` | An attack may create a false positive preventing the key to be found (try k1-17) |
| -K | Use KoreK attacks instead of PTW |
| -m `maddr` | Only keep the IVs coming from packets that match this MAC address |
| -M `num` | Specify maximum number of IVs to use |
| -n `nbits` | Set key length. 64 = `40-bit WEP`, 128 = `104-bit WEP`, etc., up to 512 (default = 128) |
| -P `num` | PTW debug: 1 Disable klein, 2 PTW |
| -s | Shows ASCII version of the key at the right of the screen |
| -t | Search binary coded decimal characters only |
| -V | Run in visual inspection mode. Can only be used when using KoreK |
| -x, -x0 | Disable last key-bytes brute-force (not advised) |
| -x1 | Enable last key-byte brute-forcing (default) |
| -x2 | Enable last two key-bytes brute-forcing |
| -X | Disable brute-force multi-threading (SMP only) |
| -y | Experimental single brute-force attack, should only be used when the standard attack fails with more than 1Mill IVs |
| -z | Use PTW attack (default) |
| -1 | Run only 1 try to crack key with PTW |

### WEP and WPA-PSK Cracking Options

| Option | Description |
| --- | --- |
| -N `file` | Create a new cracking session |
| -R `file` | Restore and continue a previously saved cracking session (this option is used alone) |
| -w `file` | Path  to a dictionary file for WPA cracking. Separate filenames with `,` when using multiple files |

### WPA-PSK Options

| Option | Description |
| --- | --- |
| -E `file` | Create Elcomsoft Wireless Security Auditor (EWSA) Project file v3.02 |
| -j `file` | Create Hashcat v3.6+ Capture file (HCCAPX) |
| -J `file` | Create Hashcat Capture file (HCCAP) |
| -r `db` | Path to the `airolib-ng` database. Cannot be used with `-w` |
| -S | WPA cracking speed test |
| -Z `sec` | WPA cracking speed test execution length in seconds |

### Input files
* Capture files: `.cap`, `.pcap`
* Hashcat HCCAPX files: `.hccapx`
* IVS: `.ivs`




