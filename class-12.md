# Chart.js, Canvas

## Chart.js

- **Chart.js** is javascript plugin that uses html5 canvas elements to draw graphs onto the page

*\<canvas>* - only supports primitive shapes

- all other shapes must be created by combining one or more paths
  
```js
function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');
// draws a clear rectangle
    ctx.fillRect(25, 25, 100, 100);
    // Draws Rectangle outline
    ctx.clearRect(45, 45, 60, 60);
    //clears teh area making rectangle transparent
    ctx.strokeRect(50, 50, 50, 50);
  }
}

```

<cite>https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes</cite>

## Drawing paths


Paths - is a list of points, is a list of segments of lines

- can be different colors
- can be curved or not curved
- paths can e closed to make shapes

#### How to make shapes

1. create path
2. use drawing command to draw into path
3. stroke or fill path to render it

### Functions Steps

beginPath() - Creates a new path

closePath() - Adds a straight lines

stroke() - draws shapes by stroking outline

fill() - fill paths content area

## colors

#### use fillStyle and strokeStyle to set color and shape

- fillStyle = color
  - sets style used when filling shapes
- strokeStyle = color
  - sets the style for shapes outline

#### Drawing text

- fillText
  - Fills in given text at given position

```js

 //fillText syntax fillText(text, x, y [, maxWidth])

function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  ctx.font = '48px serif';
  ctx.fillText('Hello world', 10, 50);
}

```
<cite>https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text</cite>


- strokeStyle

  - font 
    - same syntax as css font
  - textAlign
    - Values are start, end, left, right or center
  - textBaseline
    - Values are top, hanging, middle, alphabetic, ideographic
  - direction
    - Values are ltr, rtl, inherit
