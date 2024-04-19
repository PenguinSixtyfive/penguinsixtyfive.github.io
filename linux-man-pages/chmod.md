# CHMOD

Change file mode bits

### Modes

`chmod` follows the convention `chmod <user><operator><mode>`\

| Mode | Description |
| --- | --- |
| u | Change mode for current user |
| g | Change mode for group |
| o | Change mode for owners |
| a | Change mode for all |
| + | Adds mode to file |
| - | Removes mode from file |
| r | For `READ` rights |
| w | For `WRITE` rights |
| x | For `EXECUTE` rights |

### Common Options

| -c | Like `-v` but report only when a change is made
| -f | Suppress most error messages |
| -R | Change files and directories recursively |
| -v | Output a diagnostic for every file processed


