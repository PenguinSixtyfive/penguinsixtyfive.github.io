# RM

Remove files or directories.

### Common Options

| Option | Description |
| --- | --- |
| -d | Remove empty directories |
| -f | Ignore nonexistent files and arguments, never prompt |
| -i | Prompt before every removal |
| -I | Prompt once before removing more than three files, or when removing recursively |
| -r, -R | Remove directories and their contents recursively |

### Notes
* By default, `rm` does not remove directories.
* If you use `rm` to remove a file, it might be possible to recover some of its contents, given  sufficient expertise and/or time.
* For greater assurance that the contents are truly unrecoverable, consider using `shred`.


