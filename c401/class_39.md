# React 3

## NextJs

### Assets

Static Assets like image can be served under the top-level public directory. Files inside the public file can be referenced from the root of the application.

Nextjs handles image optimization next/image.

```js
import Image from 'next/image';

const YourComponent = () => (
  <Image
    src="/images/profile.jpg" // Route of the image file
    height={144} // Desired size with correct aspect ratio
    width={144} // Desired size with correct aspect ratio
    alt="Your Name"
  />
);
```

[Create a Next.js App](https://nextjs.org/learn/basics/create-nextjs-app)

### React Context for Beginners

React context allows us to pass down data to components we need in our React app without using props.

Context helps with props drilling

Props drilling - is when you pass props through multiple levels that do not need it

When to use context

- Theme data
- Specific user data
- Location-specific data

How to use context

- Create a createContext method
- Wrap the context provider around your component tree
- Use the value prop and put any value you like on your context provider
- Read that value within any component by using the context consumer

[React Context for Beginners – The Complete Guide (2021)](https://www.freecodecamp.org/news/react-context-for-beginners/#what-is-react-context)
