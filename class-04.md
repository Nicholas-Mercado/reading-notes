# HTML Links, JS Functions, and Intro to CSS Layout

## Links

Linking to a outside web address

```html
<a href="web address"> viewable text</a>
```

Linking within website

```html
<a href="about-me.html">About me</a>
```

Linking within website to child folder

```html
<a href="file2/about-me.html">About me</a>
```

Linking within website to parent folder

```html
<a href="file2/../about-me.html">About me</a>
```

Opening link in new window

```html
<a href="file2/../about-me.html" target="_blank'>About me</a>
```

Linking to specific part of same page

- Use Id attribute
  
```html
<a href="#top">About me</a>
```

Linking to specific part of another webpage

- Use Id attribute + web address
  
```html
<a href="http:/www.webaddress.com/#top">About me</a>
```

## Layouts

### Building Blocks

- Block level boxes
  - Start on a new line
- Inline
  - Flow between surrounding text

### Overlapping Elements

- If you use fixed or relative or absolute positioning
  - the element that appears later in code will be on top
  - use the z- index property
    - higher the number teh closer to the front
  
```css
z-index: 10;
```

### Creating Multi Columns

- Gives you two columns
- this can be done for Multi columns

```css
.column1{
  float: left;
  width: 620px;
  margin: 10px;
}

.column2{
  float: left;
  width: 300px;
  margin: 10px;
}
```

  <cite>Jon Duckett HTML & CSS: Design and Build Web Sites pg. 375</cite>

### Screen Resolution

- width: shoot for between 960-1000px
- height: Let user get strong feel for site in 570-600px

### Fixed Layout

- *Advantages*

  - px values are accurate at controlling sizes
  - control the lengths of text lines
  - size of image always the same

- __Disadvantages__

  - can have gaps
  - if user screen to high res web page can look small
  - user my not be able to increase page size
  - page most likely will take up more vertical space

### Liquid Layout

- *Advantages*

  - pages expand to fit screen
  - if user window small still fits
  - tolerant of user font sizes

- __Disadvantages__

  - if no width control page could look different
  - if user screen to high res web page can look small
  - can squish words in narrow window
  - images and text can over Flow

### Functions

- lets you have a group or series of statements perform a task

Declaring a Functions

```js
function sayHi() {
  console.log('hi')
}
//function = keyword
//sayhi() = function name
//console.log('hi') = code Block
 ```

Calling a function

```js
sayhi();
```

Declaring functions that need information

```js
function getArea(width, height){
 return width * height;
}
```

Calling a function that need information

```js
getArea(3,5);
```

You can also use variables

```js
let wallWidth = 3;
let wallheight = 5;

getArea(wallWidth, wallheight);
```
<cite>Jon Duckett HTML & CSS: Design and Build Web Sites pg. 94</cite>