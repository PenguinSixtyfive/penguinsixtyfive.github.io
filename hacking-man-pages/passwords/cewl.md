# CEWL

Custom word list generator.

`cewl`, pronounced "cool", is an app which spiders a given URL, up to a specified depth, and returns a list of words which can then be used for password crackers such as John the Ripper. Optionally `cewl` can follow external links.\
`cewl` can also create a list of email addresses found in `mailto` links. These email addresses can be used as usernames in brute force actions.

### Common Options

| Option | Description |
| --- | --- |
| -a | Include meta data |
| -c | Show the count for each word found |
| -d `x` | Depth to spider to, default = 2 |
| -e | Include email addresses |
| -k | Keep the downloaded file |
| -m `min_word_length` | Minimum word length, default = 3 |
| -w `file` | Write the output to the file |
| -v | Verbose output |
| --convert-umlauts | Convert common Latin umlauts (ä=ae, ö=oe, ü=ue, ß=ss) |
| --exclude | A file containing a list of paths to exclude |
| --lowercase | Lowercase all parsed words |
| --with-numbers | Accept words with numbers in as well as just letters |

### Notes

* Sometimes, `cewl` will return nothing. Use -v option to see the issue causing no output.
* `cewl` has options for authentication and proxies, refer to the manual for more info.


