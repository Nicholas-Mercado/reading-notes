# React and Forms

## React Docs - Forms

**What is a ‘Controlled Component’?**
A controlled element is a Component that renders forms elements and controls them by that specific data in the component state.

<cite>stackoverflow,<https://stackoverflow.com/questions/42522515/what-are-react-controlled-components-and-uncontrolled-components></cite>

**Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**

We should wait to update as the user enters them because our function handlechange updates the react state with every keystroke.

**How do we target what the user is entering if we have an event handler on an input field?**

We target the user input by setting the state to value in the handlechange function

```js

handleChange(event) {
    this.setState({value: event.target.value});
  }
```

## The Conditional (Ternary) Operator Explained

**Why would we use a ternary operator?**
Allows you to preform a if statement with less lines of code.

**Rewrite the following statement using a ternary statement:**

```js
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

The above code rewritten

```js

let z = x===y ? true : false;

```

## Things I want to know more about