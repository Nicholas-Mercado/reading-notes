# React 1

## ES6 Overview

Some fun stuff I forgot about Javascript!

Variable declaration - use var , lets , const

Arrow functions function func(a, b, c) {} --> let func = (a, b, c) => {}

Array iteration

```Javascript
for (let i of arr) {
  console.log(i)
}
```

[ES6 Overview](https://www.taniarascia.com/es6-syntax-and-feature-overview/)

## React

### **Props vs State**

Props are used to pass data from one component to another in one direction.

The state is react object that contains data and can change over time.

## Tailwind

Tailwind looks like its the answer to all the things I did not like about bootstrap.

setup:

    npm install -D tailwindcss

    npx tailwindcss init

Configure  the `tailwind.config.js` file

```Javascript
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

Add to CSS

```Javascript
@tailwind base;
@tailwind components;
@tailwind utilities;
```

build tailwind with CLI

    npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch

