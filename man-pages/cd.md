# CD

Change the working directory in the shell.

### Common Options
| Option | Description |
| --- | --- |
| -L | Force symbolic links to be followed. Resolve symbolic links in DIR after processing instances of `..`. |
| -P | Use the physical directory structure without following symbolic links.
| -e | If the `-P` option is supplied, and the current working directory cannot be determined successfully, exit with a non-zero status |

### NOTES
* The default `DIR` is the value of the `$HOME` shell variable.
* If `DIR` is `-`, it is converted to `$OLDPWD`, jumps back and forth.
* The default is to follow symbolic links, as if `-L` were specified.


