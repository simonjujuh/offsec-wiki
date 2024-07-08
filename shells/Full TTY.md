# Full TTY

```bash
# Get number of rows and columns
stty -a

# In reverse shell
python3 -c 'import pty; pty.spawn("/bin/bash")'
CTRL+Z
stty raw -echo; fg; ls; export SHELL=/bin/bash; export TERM=xterm; reset

# Use specific raws and columnes
stty rows 38 columns 116; reset
```
