# Read: 06 - JS Object Literals; The DOM

## Primitive Values vs Object References

### Primitive Values

- Data that is not a object and has no methods
- Are immutable

```html

let moe = "taco

```

### object References

- Do not contain the value just are a reference to the info
- Mutable

```html

const moe = {
  name: 'Moe Szyslak',
  occupation: 'Bartender',
  voicedBy: 'Hank Azaria'
}

```

<cite>Chris Geelhoed, What’s the Difference Between Primitive Values and Object References in JavaScript?</cite>

## Objects

- Group of sets of vairbles and functions to create a model

```js

let person = {
  firstName: "Nick",
  lastName: "Merc",
  age: 32,
  eyeColor: "blue"
};

```

### Accessing an Object

```js

let personName = person.name;

```

## The DOM

- is a tree model of a webpage pg.187

```js

//Accessing elements of the Dom single

getElementby()

querySelector()

//Selecting multiple elements

getElementsbyclassname()

getElementsbyTagName()

querySelectorAll()

```

### Traversing the Dom

- move form node to node

```js
.parentnode

.previous or nextSibling

.firstchild, .lastChild
```

*Do not use innerHTML*

Traversing the dom can be tricky because some browsers add whitespace.
This is why we use libraries like jQuery
