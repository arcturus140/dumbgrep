## dumbgrep
A Python implementation of grep, which can be used as a template for CLI tools.

Accompanying article: [Recreating grep in Python](https://kevingal.com/blog/cli-tools.html) (working title).

Usage:

```
$ dumbgrep existence </tmp/war-and-peace.txt
in this part of the house and did not even know of the existence of
even wish to know of his existence but would now have been offended
[...]
$ dumbgrep -h
usage: __init__.py [-h] [-v] [--max-count MAX_COUNT] pattern

A replacement for grep.

positional arguments:
  pattern               the pattern to search for

optional arguments:
  -h, --help            show this help message and exit
  -v                    invert matches
  --max-count MAX_COUNT, -m MAX_COUNT
                        max number of matches to print
```

## Packaging

```bash
python3 setup.py sdist
```

## Installation

`python3 setup.py install`
`python3 setup.py develop`

or

`pip3 install .`


## Deploy

```bash
python setup.py register
python setup.py sdist upload
```
