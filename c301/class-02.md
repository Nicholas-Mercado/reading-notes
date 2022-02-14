# State and Props

## React lifecycle

**Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**

The render

**What is the very first thing to happen in the lifecycle of React?**

**Mounting** - When a instance of a component is created and inserted in the DOM

**Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates**

1. constructor
2. render
3. React Updates
4. componentDidMount
5. render
6. React Updates
7. componentWillUnmount


**What does componentDidMount do?**

Allows for us to execute code when the component is already placed in the DOM

## React State Vs Props

**What types of things can you pass in the props?**

Like arguments to a function. When you want to display information without hard coding it.

- What you want you component to render like
  - title, sub title etc..
- initial data

**What is the big difference between props and state?**

Props are handles outside of a component. State is handled inside a component and can be updated inside that specific component

**When do we re-render our application?**

When you change a state.

**What are some examples of things that we could store in state?**

If you need to re-render or update your application based on what the user has done.

Storing a update for a form input element by a user

## Things I want to know more about
I am interested in seeing how state handles events
