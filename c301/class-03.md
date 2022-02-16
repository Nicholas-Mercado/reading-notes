# Passing Functions as Props

## React Docs - lists and keys

**What does .map() return?**
map() returns a new array populated with the results of a function on each element of a array you called

**If I want to loop through an array and display each value in JSX, how do I do that in React?**
You can loop through and array and display each value by using {}. see code below for example

```js

const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li> // enclose value in {}
);

```

<cite>Rendering Multiple Components, "https://reactjs.org/docs/lists-and-keys.html"</cite>

**Each list item needs a unique **Key**.**

**What is the purpose of a key?**

A **Key** helps React identify which items have changed

## The Spread Operator

**What is the spread operator?**

is the use of (...) to expand an iterable object into a list of arguments

**List 4 things that the spread operator can do.**

1. Spreads array into separate arguments

2. Copy an array

3. Add state in React

4. combine objects

**Give an example of using the spread operator to combine two arrays.**

```js

const arr1 = ['2','3','4']
const arr2 = ['7','5','6']
const arr3 = [...arr1,...arr2]

```

**Give an example of using the spread operator to add a new item to an array.**

```js
const arr1 = ['2','3','4']
const add = ['12','10', ... arr1]

```

**Give an example of using the spread operator to combine two objects into one.**

```js
const obj1 = {hi:"1"}
const obj2 = {hello:"3"}
const obj3 = {...obj1,...obj2}

```

## How to Pass Functions Between Components

**In the video, what is the first step that the developer does to pass functions between components?**

```js
increment = (name) =>{
 // the dev had to use increment to pass functions to parent
 }
```

**In your own words, what does the increment function do?**
The increment function increases or decreases a given value.

**How can you pass a method from a parent component into a child component?**

You can pass a method from parent to child element by calling the function with the this keyword in the component object.

```js
increment={this.increment}
```

**How does the child component invoke a method that was passed to it from a parent component?**

This invokes the method in the parent element casuing a rerender and changing state.

```js
this.props.increment(this.props.name);
```

## Things I want to know more about
