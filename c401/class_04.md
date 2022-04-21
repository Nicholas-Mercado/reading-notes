# Topic: Class 04

## Classes and Objects

Objects groupings of variables and functions into a single entity

Classes are a template to create your objects

Each object contains independent copies of the variables defined in the class

__init__() -  function, is a special function that is called when the class is being initiated.

[Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)

## Thinking Recursively

If the problem is simple just solve it. Otherwise break it down into sub problems

A recursive function is a function defined in terms of itself via self-referential expressions.

Recursive functions share a common structure made up of two parts

- base case

- recursive case

[Thinking Recursively in Python](https://realpython.com/python-thinking-recursively/#dear-pythonic-santa-claus)

### Maintaining State

To maintain state during recursion you have to either:

- Thread the state through each recursive call

- Keep the state in global scope
  
[Maintaining State,Thinking Recursively in Python](https://realpython.com/python-thinking-recursively/#dear-pythonic-santa-claus)

global mutable state is evil

## Recursive Data Structures in Python

A data structure is recursive if it can be defined in terms of a smaller version of itself.

## Pytest Fixtures and Coverage

Fixtures - objects can contain data you want to share across tests

## Fixture errors

 Error - does not mean test fail but test could not preform

 Its a good idea to cut out as many unneeded dependencies
