# SHRED

Overwrite a file repeatedly to wipe its contents.

### Common Options

| Option | Description |
| --- | --- |
| -f | Change permissions to allow writing if necessary |
| -n | Overwrite `n` times instead of the default 3 |
| -s | Shred this many bytes (suffixes like `K`, `M`, `G` accepted) |
| -u | De-allocate and remove file after overwriting |
| -x | Do not round file sizes up to the next full block, this is the default for non-regular files | 
| -z | Add a final overwrite with zeros to hide shredding |

### Notes

* If `FILE` is `-`, shred standard output.
* **CAUTION**: `shred` assumes the file system and hardware overwrite data in place.

### [Back](linux-man-pages.md)
