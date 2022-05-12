# Automation

## Python Regular Expressions Tutorial

Dont for get to imppoirt

```py
import re
```

Uasing Ordinary Characters

setup pattern and sequence
```py
pattern = r"Cookie"
sequence = "Cookie"
```

use re.match to check for match

```py
if re.match(pattern, sequence):
```

useful re methods

- search() - finds the first location where the re produces a match
- group() - returns the string matched by the read

useful regex

- . matches any single single character except the newline character
- ^ matches start of the string
- \- matches the end of a string
- \* the character is repeated zero or more times
- \+ the character is repeated at least once
- \{} character is repeated as many times as mentioned in the braces
- ? character is optional
- $ match must occur at end of string
- [] match one out of all Characters within brackets
  

[Python Regular Expression (RegEX)](https://www.simplilearn.com/tutorials/python-tutorial/python-regular-expressions)

### Basic patterns

## shutil

Shutil is a module that facilitatres operations such as copying and archiving.

module includes high-level file operations such as copying and archiving.

how to import

```Python
import glob
import shutil

```

## useful methods

copyfile() - coppies content of source to destination but will raise error if it does not have permission

copy() - if the named destination is a folder, will create new file

copymode() - copies permissions from one file to another
