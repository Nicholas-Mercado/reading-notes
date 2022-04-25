# Ten Thousand 2

## Scope

Scope - are the rules on how variables are looked up in your

### LEGB

LEGB - stands for local, Enclosing, Global and Built-in.

#### **Local**

- or Function levels
- These are created at function call not function definition

#### **Enclosing**

- or non local scope
- only exists for nested functions
- contains named are available all Enclosing functions

#### **Global**

- or module scope
- contains all names defined at the top levels

#### **Built-in**

- created when ever you run a script
- contain all pre loaded python keywords, function...


Global Scope - variables are available to all your code

local Scope - only available to code in scope

## Namespaces

Namespaces - dictionary that python uses to store variable Namespaces

When you use a name python searches different levels of scope or namespaces.

If it does not find it it creates

Else it returns first occurrence

## Global and nonlocal keywords

### global

global statement - used to define a list of names that can be used as global names

```py
counter = 0  # A global name
def update_counter():
     global counter  # Declare counter as global
     counter = counter + 1  # Successfully update the counter
```

### nonlocal

nonlocal keywords

- Can be accessed from inner functions
- cannot be used outside of the nested or enclosed function
  
```py
def func():
...     var = 100  # A nonlocal variable
...     def nested():
...         nonlocal var  # Declare var as nonlocal
...         var += 100
```

<cite>Real Python, Modifying the Behavior of a Python Scope https://realpython.com/python-scope-legb-rule/#modifying-the-behavior-of-a-python-scope</cite>
