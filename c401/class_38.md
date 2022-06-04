# React 2

## Conditional Rendering

You can create distinct components and render only the ones you need.

Use a conditional operator or if to create elements that represent current state.

```Javascript
function Greeting(props) {
  const isLoggedIn = props.isLoggedIn;
  if (isLoggedIn) {   // <<<----- if logged in get custom greeting
    return <UserGreeting />;
  }
  return <GuestGreeting />;
}

const root = ReactDOM.createRoot(document.getElementById('root')); 
// Try changing to isLoggedIn={true}:
root.render(<Greeting isLoggedIn={false} />);
```

[Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)

## Lists and Keys

Building a basic components list

```Javascript
unction NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    <li>{number}</li>
  );
  return (
    <ul>{listItems}</ul>
  );
}

const numbers = [1, 2, 3, 4, 5];
const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(<NumberList numbers={numbers} />);
```

Assigning a key

keys help react identify when and which a item has changed. Give keys to a element inside the array. If no stable ID yoy may use item index.

```Javascript
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li key={number.toString()}>
    {number}
  </li>
);
```

[Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)

## Lifting State Up


When multiple components need to share state you can lift that state to a common ancestor.

[Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)
