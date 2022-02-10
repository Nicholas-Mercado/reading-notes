# CSS Layout

## Building blocks

- **block-level** elements start a new line
- **Inline elements** flow between surrounding text
- **container elements** is block-level element with another block-level element inside

## Creating multi columns

```css
 /* I like the naming */
.column1of2 {
  float: left;
  width: 500px;
  margin:200px;
}
.column2of2 {
  float: left;
  width: 500px;
  margin:200px;
}
```

<cite>Jon Duckett, HTML and CSS: Design and Build Websites pg 375</cite>

## Multicolumn layout

```js
<h1>All countries</h1>
<ul class="countries">
  <li>Argentina</li>
  <li>Aland Islands</li>
  <li>Albania</li>
  <li>Algeria</li>
  <li>American Samoa</li>
  <li>Andorra</li>
</ul>

.countries {
	column-count: 2;
	column-gap: 1em;
}

```

<cite> https://web.dev/learn/css/layout/ </cite>

## Flexbox vs Grid layout

### Flexbox

- for one-dimensional layouts across a single access
- will align elements children to each other in the inline direction
- all elements will be same height

### Grid

- similar to flexbox but designed to control multi access layouts
- Allows you to write layout rules on a element
- introduces new primitives for layout styling
  - repeat()
  - minmax()
- fr is a unit measuring a fraction of remaining space

```css

.my-element {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  gap: 1rem;
}

```



