# FileIO & Exceptions

## Read & Write Files in Python

Useful things I learned in this article

The double-dot (..) can be used to move one directory up.

The double-dot (..) can be chained together to move up as many directories as you want ../../ 

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

Syntax errors - when the parser detects a incorrect  statement

Exception error - This occurs when syntactically correct code results in error

### Raising an Exception

  we can use raise to throw a custom Exception

```py
x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))
```

### The AssertionError Exception

AssertionError - set a parameter that cannot be used broken for the code to run

```py
assert ('linux' in sys.platform), "This code runs on Linux only."
```

### The try and except Block

try and except - are used to catch and handle exceptions 

```py
try:
  this code
except:
  run this code if exception
```

You can use this to continue the program without crashing while adding a note for the user

Warning: Catching exception hides errors. Its best practice not to use bare except clauses

### The else Clause

With the Else statement you can have python execute code only in absence of exceptions

```py
try:
  this code
except:
  run this code if exception
else: 
  only ran if no exceptions
```

### Cleaning Up After Using finally

finally - allows you to always run code.

```py
try:
  this code
except:
  run this code if exception
else: 
  only ran if no exceptions
finally:
  Always run this code
```
