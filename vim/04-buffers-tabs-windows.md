# Buffers, tabs & windows

Like any other text editor, Vim can work with multiple files at once, called `buffers`.

### Buffers
| Key combo | Command |
| --- | --- |
| :e | Edit file in new buffer |
| :ls | view files in buffer |
| :bp | Go one file back (buffer previous) |
| :bn | Go one file forward (buffer next) |
| :bd | Remove file from buffer (buffer delete) |

### Tabs:
| Key combo | Command |
| --- | --- |
| :tabedit <file> | Edit file in new tab |
| :tabe <file> | Edit file in new tab |
| :tabp | Previous tab |
| :tabn | Next tab |
| :tabm | Move tab |
| :tabnew | new tab |
| :tabonly | close all tabs not in focus |

### Splits:
| Key combo | Command |
| --- | --- |
| :sp | Split |
| :vsp | Vertical split |
| C-w arrow | Navigate between splits |
Where `C` is `ctrl`.

### Sessions:
A Vim session is a collection of files saved together.
| :mksession <file>.vim | Save multiple files as a vim session |



