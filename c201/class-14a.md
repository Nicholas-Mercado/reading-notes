# CSS Transforms, Transitions, and Animations

## Transforms

**Transforms** come in two diffrent settings

- two-dimensional
- three-dimensional

### Transform Syntax

```css
div {
  /* //Use multiple prefixs to gain support from browsers */
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```

<cite>https://learn.shayhowe.com/advanced-html-css/css-transforms/</cite>

## Transitions & Animations

**Transforms** 

- Change the appearance and behavior of an element when a state change occurs
  - hover
  - focused on
  - active
  - target

### Transition Properties

- transition-property
- transition-duration
- transition-timing-function
- transition-delay

```css
.box {
  background: #2db34a;
  /* Select the background */
  transition-property: background;
  /* how long for transition */
  transition-duration: 1s;
  /* Sets intermediate values */
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
```
<cite>https://learn.shayhowe.com/advanced-html-css/transitions-animations/</cite>

## Animations

- When transition need multiple states

**Keyframes** - set multiple points at which an element should undergo a transition

```css
@keyframes slide {
  /* Three breakpoints are set as % */
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
```

<cite>https://learn.shayhowe.com/advanced-html-css/transitions-animations/</cite>