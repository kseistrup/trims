# TRIMS

Trims Redundant Input, Merges Services

## Usage

```txt
Usage: trims [OPTIONS] [SERVICES [SERVICES …]]

positional arguments:
  SERVICES              services(5) compliant input file

optional arguments:
  -h, --help            show this help message and exit
  -v, --version         show version information and exit
  -c, --copyright       show copying policy and exit
  -o OUTPUT, --output OUTPUT
                        resultant services(5) compliant file

Trims trims one or more services(5) compliant files such that
the result has exactly one line for each unique port/protocol
combination. In short, a union of all combinations seen.

If no filenames are given on the commandline, or if the pseudo
filename ‘-’ is used, standard input is assumed.

Services from files that appear later on the commandline takes
presedence over data from earlier files. In this case earlier
service names are moved to the aliases list.

The result is written to standard output unless an output file
is given explicitly, using the ‘-o’ / ‘--ouput’ option.
```

:smile:
