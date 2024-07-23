# bash-prompt-stuff

## Adding timestamps to bash

```
# For bash prompt itself
export PROMPT_COMMAND="echo -n \[\$(date +%H:%M:%S)\]\ "
# For .bash_history
export HISTTIMEFORMAT="%d/%m/%y %T "
```

## History Searching

```
# Inside ~/.inputrc
$ cat ~/.inputrc
"\e[A": history-search-backward
"\e[B": history-search-forward
```

This allows one to type a partial command and press up and down arrow keys to navigate history.
