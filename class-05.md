# Html Images; CSS Color & Text

## Images

### Images should

- be relevant
- convey info
- fit the color pallette

### Control width and height

```html

<img src="" width="600" height="405'>

```

```Html
<figure>
  <figcaption>THis is a caption
  </figcaption>
  // two tags required, source (src), alt for screen readers
  // can have tag Title
  <img src="weblocation" alt="Html-simple-description" title="name of image">
</figure>  

```

### Three rules for creating Images

- Save images in the right format
- Save images at the right size
- Measure images in pixels
  
<cite>Jon Duckett</cite>

## Color

Use color to set the mood of your site. Keep in mind images you will use when choosing color pallette

### Contrast

- When choosing colors make sure there is enough contrast to make text legible

- If text is light on dark background increase line height for legibility

### Hsl

- hue is expressed in 360 degrees
- Saturation is in %
- lightness is in % 0%-white 50%-normal 100%-black

```css

hsl(0,50%,78%)

```

## Text

### Changing fonts

Font stack

- letter-spacing:

- font-family: has small list of fonts so website can use at least one

Font-face

- allows you to specify a path and the users computer will dl if not on already
  
Leading

- Pronounced *ledding*
- Is the height between lines fo type
- use the line-height property to change

## __JPEG vs PNG vs GIF__

### JPEG

- Pros
  - Very Compatible
  - widespread use
  - quick loading
  - full color spectrum

- Cons
  - lossy compression
  - no animations
  - no transparency
  - no layer

### PNG

- Pros

  - lossless compression
  - supports semi transparency
  - full color spectrum

- Cons
  - Not good for print
  - more memory
  - not universally supported
  - No animations

### GIFS

- Pros
  - good for simple animations
  - small file size
- Cons
  - limited color
  - web only
