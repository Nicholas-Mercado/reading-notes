# Object-Oriented Programming, HTML Tables

## Html Tables

### Tables

- represents information in a grid from
- allows you to understand complex data
- represented on two axes
  
### Basic table structure

```html

<table>
  <tr>
    <td>1</td>
    <td>2</td>
    <td>3</td>
    <td>4</td>
  </tr>
  <tr>
    <td>5</td>
    <td>6</td>
    <td>7</td>
    <td>8</td>
  </tr>
  <tr>
    <td>9</td>
    <td>1</td>
    <td>1</td>
    <td>1</td>
  </tr>

// shown like This
1 2 3 4
5 6 7 8
9 1 1 1
```

**tr** - starts a row

**td** - is a single cell

**th** - represents heading to a column

```html

<table>
  <tr>
    <th></th> // empty place holder
    <th>Saturday</th>
    <th>Sunday</th>
  </tr>
  <tr>
    <th>Tickets sold</th>
    <td>120</td>
    <td>30</td>
  </tr>
// shown like This

              Saturday Sunday
Tickets sold    120     30

```

<cite> Jon Duckett, HTML & CSS: Design and Build Web Sites </cite>

## Functions, Methods, and Objects

### Creating many Objects

- you can use a function to template Objects

```js

function person(firstName,lastName, age){
  this.firstName = firstName;
  this.lastName = lastName;
  this.age = age;
};

// Creating new object from object function

ver = Nicholas = new person('Nicholas','Mercado','35');

```

### Built in Objects

#### There are three groups of built in Objects

- Browser Object Modeling
- Document Object Modeling
- Global JavaScript Objects

#### Browser Object Model

- is the model for browser tab or window

- top object is the windows
  - its child objects are
    - Document
    - History
    - Location
    - Navigation
    - Screen

#### Document Object Model

- This creates a model of your current webpage

- top object is the Document
  - its child objects are all the parts of the html
    - \<body>
    - \<div>
    - \<title>
    - etc...
  
#### Global JavaScript Objects

- Is not a single model but a group of related objects

- these objects are basic data structures
  - string
  - boolean
  - number

- these objects deal with real world concepts
  - Date
  - Time
  - etc...
