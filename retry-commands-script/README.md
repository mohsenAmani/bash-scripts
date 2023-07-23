# simple-retry commands-script

A simple retry commands script to run any command for any time and at the end return executed command status.

## How to use:

```bash
Usage: retry [OPTIONS] COMMAND
Options:
    -h: Show this help output
    -v: Verbose mode 
    -n: Number of tries (Default: 5)
    -i: Interval seconds (Default: 10)
```

### Example:

```bash
retry -v true
retry -v -n 3 -i 2 true
retry -v -i 5 true
retry -i 5 -n 2 [ -f ./test ]
```
