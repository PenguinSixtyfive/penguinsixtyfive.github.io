# MV

Move and rename files.

### Common Options

| Option | Description |
| --- | --- |
| -b | Backup but does not accept an argument |
| -f | Do not prompt before overwriting |
| -i | Prompt before overwrite |
| -n | Do not overwrite an existing file |
| -t | Move all `SOURCE` file arguments into `DIRECTORY` |
| -u | Move only when the `SOURCE` file is newer than the destination file *or* when the destination file is missing |
| -v | Explain what is being done |

### Notes

* If you specify more than one of `-i`, `-f`, `-n`, only the final one takes effect.

### [Back](linux-man-pages.md)
