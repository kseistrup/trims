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

Trims merges one or more services(5) compliant files such that
the result has exactly one line for each unique port/protocol
combination.

If no filenames are given on the commandline, or if the pseudo
filename ‘-’ is used, standard input is assumed.

Data from later files takes presedence over data from earlier
files. In this case earlier service names are added as aliases.

The result is written to standard output unless an output file
is given explicitly, using the ‘-o’ / ‘--ouput’ option.

It is safe to use the same filename for SERVICES and OUTPUT.

Trims could be a recursive acronym for Trims Redundant Input,
Merges Services.
```

:smile:
