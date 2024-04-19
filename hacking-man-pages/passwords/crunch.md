# CRUNCH

Generate wordlists from a character set.

### Common Options

| Option | Description |
| --- | --- |
| -b `number type` | Specifies the size of the output file |
| -c `number` | Specifies the number of lines to write to output file |
| -d `numbersymbol` | Limits the number of duplicate characters
| -e `string` | Specifies when crunch should stop early |
| -f `file.lst` `charset-name` | Specifies a character set from the `file.lst` |
| -i | Inverts the output, so instead of `aaa,aab,aac,aad`, etc you get `aaa,baa,caa,daa,aba,bba` |
| -l | With `-t` option this option tells crunch which symbols should be  treated  as  literals
| -m | Merged with `-p`. Please use -p instead |
| -o `wordlist.txt` | Specifies the file to write the output to |
| -p `charset` OR `-p w1 w2 ..` | Generate words that don't have repeating characters |
| -q `file.txt` | Read `file.txt` and permute what is read. Like `-p` but gets input from `file.txt` |
| -r | Resume generate words from where it left off. Only works with `-o` |
| -s `startblock` | Specifies a starting string, eg: `03god22fs` |
| -t `@,%^` | Specifies a pattern (RegEx) |
| -u | Disables the `printpercentage` thread. This should be the last option |
| -z `file.zip` | Compresses the output from the `-o` option.  Valid parameters are `gzip`, `bzip2`, `lzma`, and `7z` |

### Notes

* In RegEx: `@` is lower case characters, `,` = upper case characters, `%`= numbers, `^` = symbols.
* `crunch` supports the `space` character on the command line and in the `charset.lst`.\
To add a space on the command line you must escape it using the `/` character.
* When using `-z 7z`, `7z` doesn't delete the original file. You will have to delete those files by hand.
* For use cases and examples, refer to the manual.
* You can use crunch's output and pipe it into other programs.\
The two most popular programs to pipe crunch into are: `aircrack-ng` and `airolib-ng`. The syntax is as follows:
```bash
crunch 2 4 abcdefghijklmnopqrstuvwxyz | aircrack-ng /root/Mycapfile.cap -e MyESSID -w-
```
OR
```bash
crunch 10 10 12345 --stdout | airolib-ng testdb -import passwd -
```


