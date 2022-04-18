# Testing and Modules

## In Tests We Trust - TDD with Python

You can use unit tests to check the input and expected output of code

It is ideal to separate your tests from your production code

### Arrange, Act and Assert

- Arrange: Organize the data that will be inputted

- Act: Execute the code being tested

- Assert: Does the output match what you expected

### The Cycle

A very simple cycle that contains three steps

- Write a unit test and make sure it fails

- Write code that make it pass the test

- Refactor the code

<cite>Ana Paula Gomes,In Tests We Trust — TDD with Python,<https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932/></cite>

## If name equals main

propper format ints

```py

if __name__ == “__main__”:

```

Allows the interpreter to import a python file without running it.

## Recursion

N has many values

### Finding sum of first natural numbers

First approach : Iteratively

```c++
f(n) = 1 + 2 + 3 +……..+ n
```

Second approach : Recursively

```c++
f(n) = 1             n=1

f(n) = n + f(n-1)    n>1
```

```C
int fact(int n)
{
    if (n < = 1) // base case
        return 1;
    else    
        return n*fact(n-1);    
}
```

<cite>Sonal Tuteja,Recursion,<https://www.geeksforgeeks.org/recursion/></cite>

## Things I want to know more about

Definitely interested in learning more about unit test and making them work for me.
