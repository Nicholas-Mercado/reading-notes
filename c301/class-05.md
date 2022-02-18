# Putting it all together

## React Docs - Thinking in React

**What is the single responsibility principle and how does it apply to components?**

It is the idea that a components should only do one thing and if it grows larger then that one thing, it should be broken down in to sub components

**What does it mean to build a ‘static’ version of your application?**
To build a static version of your application is to build your data model without any interactivity ie state.

**Once you have a static application, what do you need to add?**
You need to find the minimal set of mutable state that your app requires. Keep your code very dry.

**What are the three questions you can ask to determine if something is state?**

1. Is it passed from parent via props
2. Does it remain unchanged over time
3. Can you compute it based on any other state or props in your component

**How can you identify where state needs to live?**

First list all components that render something based on that state. Then find a common owner component (a single component about all components that need state in the hierarchy) <--- I dont understand this. Either the common owner or another owner high should own the state. If one cannot be found a new component should ber created.

<cite>Thinking in React,https://reactjs.org/docs/thinking-in-react.html</cite>

## Higher-Order Functions

**What is a “higher-order function”?**
Functions that operate on other functions either by taking in arguments or by returning them

**Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?**
The greaterThan function is checking wether the the argument n is greater then m

**Explain how either map or reduce operates, with regards to higher-order functions.**
map() applies a function for us producing a new array that is the same length and only containing the content map has effected. This creates dryer code vs us building the loop ourselves therefore it will most likely contain less bugs

<cite>Higher-order functions,https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK</cite>

## Things I want to know more about

I think I would like to see someone work through static to interactivity as a demo
