## Future plans

### Ideas

## Improvements for using ‘-’ for standard IO

Using `/dev/stdin` and `/dev/stdout` as filenames for stdio works well
on unices that has these filenames — e.g., Linux. Perhaps we could use
the following workaround to increase portability (and I am not talking
about Windows here):

```py
import sys
import os

# Instead of open('/dev/stdin', 'r')
stdin = open(os.dup(sys.stdin.fileno()), 'r')

# Instead of open('/dev/stdout', 'w')
stdout = open(os.dup(sys.stdout.fileno()), 'w')
```

### Suggestions

If you feel something is missing, please open an issue on
[Github](https://github.com/kseistrup/trims/issues).
