# Basics of HTML, CSS & JS

## HTML tags
- sup
  - adds a super script
    - 4<sup>7</sup>
- sub
  - adds a subscript
    - 4<sub>7</sub>

## Semantic Markup 
- do not effect structure of the paige but add information
  - like bold, italics ...effect
- strong for bold
- em for italics
- blockquote
  
  ```html
  <blockquote cite="link">
    <p>This is the quote</p>
  ```

## intro CSS
- Think of boxes around every element

### Declarations
  - Made up of two parts
    - properties
      - background-color
    - values
      - the color ex red

## Basic Javascript instructions
- java is case sensitive!

```js
var today = new Date(); // Statement
var hourNow today. getHours () ; // Statement
var greeting; // Statement
if (hour Now 18) { //Determines which code should run
greeting = "Good evening"; // Statement
} else if (hourNow 12) { //Determines which code should run
greeting = "Good afternoon" ; // Statement
} else if (hourNow 0) { //Determines which code should run
greeting = "Good morning" // Statement
} else { //Determines which code should run
greeting = "Welcome"; // Statement
document. write (greeting); // Statement
```
<cite>JavaScript and JQuery: Interactive Front-End Web Development by Jon Duckett</cite>

### multi line comment
```js
Use /*  to write multi line comments */
```

### Declaring a Variable

```js
name = 3;
```
Variable name , assignment operator, variable values
### rules for naming vaiables
  - must begin with letter, doller sign, or underscore
  - name may only contain letters, number, dollar sign or underscore
    - no . or -
  - cannot use keywords or reserved words
  - are case sensitive
  - use a name that describes information stored
  - if more then one word use capital to distinguished

## Creating a Array\
- arrey numbering starts at 0
```js
let colors = new Array('go','left','foot');
```
## Accessing a changing a arrey

```js
//Create the array
var colors ['whi te',
'black',
'custom']:
//Update the third item in the array
colors[2] = "beige";
//Get the element with an id of colors
var el= document.getElementById ('colors');
// Replace with third item from the array
el.textContent = colors [2];
```
<cite>JavaScript and JQuery: Interactive Front-End Web Development by Jon Duckett</cite>

