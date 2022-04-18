# FileIO & Exceptions

## Read & Write Files in Python
Useful things I learned in this article

You can use the special characters double-dot (..) to move one directory up.--

The double-dot (..) can be chained together to traverse multiple directories above the current directory. ../../ --

Opening a file and closing file

```py
file = open('myfile.txt')
reader.close()
```

Using with statment to open and close file

```py
with open('myfile.txt') as reader: 
``` 

3 methods for reading a file

- .read() - reads whole file
- .readline() - reads a most size of line passed in argument
- .readlines() - reads remaining lines in file - returns list

## Exceptions in Python
