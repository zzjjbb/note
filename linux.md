# General Linux Note

## SSH

Interactive: `ssh -t 127.0.0.1 python`

## Bash

### login shell

Use `bash -l`

Example:

```sh
#!/bin/bash -l
# your script
```

### heredoc

Main application: write block/multiline content to some file

```sh
<< EOFFFF > sy.txt
line 1
$TERM
EOFFFF
```

content in sy.txt:

```
line 1
xterm (maybe)
```

Change the beginning of the 1st line to `<< "EOFFFF"` or even
`<< E"OF"FFF` or `<< EO'F'FFF` to get the raw string `$TERM` in the 2nd
line of `sy.txt`.
