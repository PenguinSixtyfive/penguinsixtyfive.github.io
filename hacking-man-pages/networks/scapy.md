# SCAPY

Interactive packet manipulation tool

### Common Options

| Option | Description |
| --- | --- |
| -C | Do not run startup file |
| -d | Increase log verbosity. Can be used many times |
| -H | Header-less mode, also reduces verbosity |
| -P | Do not run pre-start file |
| -s `file` | Use `file` to save/load session values (variables, functions, instances, ...) |
| -p `prestart-file` | Use `file` instead of `$HOME/.config/scapy/prestart.py` as pre-startup file |
| -c `starup-file` |Use `file` instead of `$HOME/.config/scapy/startup.py` as startup file |

### Commands

* Only the vital commands to begin are listed here for the moment.
* `conf`: This object contains the configuration.
* `lsc()`: Lists `scapy`'s main user commands.
* `ls()`: lists supported protocol layers.\
If a protocol layer is given as parameter, lists its fields and types of fields.\
If a string is given as parameter, it is used to filter the layers.

### Files

1. `$HOME/.config/scapy/prestart.py`:
* Runs before `scapy` core is loaded.
* Only the conf object is available.
* Can be used to configure the CLI & parameters such as `conf.load_layers` list to choose which layers will be loaded,\
or change the logging level (for instance):

```bash
conf.interactive_shell = "bpython"
```

```bash
log_loading.setLevel(logging.WARNING)
```

```bash
conf.load_layers.remove("bluetooth")
```

```bash
conf.load_layers.append("new_layer")
```

2. `$HOME/.config/scapy/startup.py`:
* This file is run after `capy` is loaded.
* It can be used to configure more of `scapy` behaviors, like unregistering layers:

```bash
conf.prog.pdfreader = "xpdf" 

split_layers(UDP,DNS)
```


