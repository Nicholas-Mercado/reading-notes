# HTML Lists, Control Flow with JS, and the CSS Box Model

## __Lists__

### 3 types of Lists
  - unordered
  - ordered 
  - definition 

#### Ordered and unordered
  - both have li nested in them
    - \<li>
  - Ordered list denoted
   1. test 
   2. test 
   3. test
  - Unordered list denoted
    - .
    - .
    - .
  
#### Definition lists
- created with dl element
- use dt for term
- use dd for Definition


```md

<dl>
  <dt>dog</dt>
  <dd>mans best friend</dd>
</dl>

```

## Boxes

### box dimensions
  - width
  - height
  - use em, px, or %

### Limiting Width
- min-Width
- max-Width
  - use these to control how large and small a box will become depending on browser window.

### Padding
- how much space between content of element and border
- Shorthand: padding: (top, right, bottom, left)
  -  padding: 1px 2px 3px 4px;


### Margin
- How much space between elements
-  Shorthand: margin: top, right, bottom, left
   -  Margin: 1px 2px 3px 4px;
-  Shorthand: margin: topbottom, rightleft
-  Margin: 1px 2px;

## Creating a Array
- arrey numbering starts at 0
  
```md

let colors = new Array('go','left','foot');

```

## Accessing a changing a array

```md
//Create the array
let colors ['whi te',
'black',
'custom']:
//Update the third item in the array
colors[2] = "beige";
//Get the element with an id of colors
let el= document.getElementById ('colors');
// Replace with third item from the array
el.textContent = colors [2];
```

<cite>JavaScript and JQuery: Interactive Front-End Web Development by Jon Duckett</cite>

## __Switch Statements__
  - peforms faster then if Statements
  
```md
  switch (expression) {
  case value1:
    [break;]
  case value2:
    [break;]
  case valueN:
    [break;]
  [default:
    [break;]]
  }
```

  [MDN Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch)

## Coercion
  - JavaScript may convert data behind the scenes to try to make sense of data it did not expect

```md
('1'>0) 
```

- js may convert the 1 into a number from a string

## *Using for loops*


```

let scores [24, 32, 17]; //Array of scores
let arrayLength = SCores.length;// Items in array
let roundNumber 0; //Current round
let msg ''; //Message
let i; // Counter

//Loop through the items in the array
for (i = 0; i < arrayLength; 1++) {

//Arrays are zero based (so 0 is round 1)
//Add 1 to the current round
roundNumber = (i + 1);

//Write the current round to message
msg+ "Round+ roundNumber+':'

//Get the score from the scores array
msg+= scores [i] + '<br />';
document.getEl ementByI d ( 'answer').innerHTML = msg;
```


<cite> Jon, Duckett JavaScript & jQuery
Interactive Front-end Web Development</cite>