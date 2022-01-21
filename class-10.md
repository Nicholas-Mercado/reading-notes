# JS Debugging

## Execution Contexts

- **Global** Contexts
  - Code that is in the script but not in a function
- **function** Contexts
  - Code that is run in a function
  - each function has its own Contexts
- **Eval** Contexts
  - text executed like code in a internal function
    - not seen

### variable Scope

- Global Scope
  - if a variable is declared outside a function it can be used anywhere

- function level Scope
  - when a variable is declared in a function it can only be used in that function

## THe Stack

Javascript read code one line at a time. So when a statement needs data from another function it stacks or piles the new function on current one.

- Each time a new item is added to the stack it creates a new execution Contexts

### _Hoisting_

- Variables  are hoisted to the top of the block, but not initialized.

- Allows the call of function before they are declared

- Assigns a value to a variable that has not been declared

```js 
//This will not work
carName = "Volvo";
let carName;
```

<cite>w3schools,https://www.w3schools.com/js/js_hoisting.asp </cite>

## Error Objects

### Chrome browser error msgs

- error
  - Generic error
- syntax
  - incorrect use of language, often a typo
  - missing brackets
  - unclosed quotes or mismatching
- Reference
  - Caused by a variable that is undeclared or out of scope
  - function is undefined
- type
  - often caused by trying to use a object or method that doesn't exist
- Range
  - calling a function using numbers outside of its excepted range
- URI
- If special characters are not escaped in URI they will cause error
  - / ? & # : ;
  