# Pythonisms

## Dunder Methods

Dunder or magic methods - set of predefined methods used to enrich your classes

dunder methods are used to mimic built in functions

Object Representation:

- __repr__ - Formal string representation
- __str__ - Informal representation


Comparing Object Instances:

- __eq__ - Returns true if equal
- __lt__ - Returns true if less then

[Dunder method list](https://holycoders.com/python-dunder-special-methods/)

## Iterators

Iterators 

- is a object that contains a countable number of values
- is a object where you can traverse through all the values
- contains __iter__() and __net__()

Iterable objects

All of these objects contains a iter()

- list
- tuples
- dictionaries
- sets


[Python Iterators](https://dbader.org/blog/python-iterators)

[Iterators](https://www.w3schools.com/python/python_iterators.asp)

## Generators

Generator - is like a normal function but contains a yield statement

- Local variables and states are remembered between calls
- `StopIteration` is raised automatically

yield - does not terminate function just pauses it.


[Python Tutorial: Generators](https://www.youtube.com/watch?v=bD05uGo_sVI)
