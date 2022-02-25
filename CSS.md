# CSS : Cascading Style Sheets
## Outline
- Adding CSS to the document
- Basic selectors(HTML elements, class, id)
- Advanced selectors
- Properties and values

# Adding CSS to the document
[Getting started with CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/Getting_started)

Add the link tag to the head of the html file
```html
<link rel="stylesheet" href="styles.css">
```

# Basic selectors (HTML elements, class, id)
## Styling HTML elements

```css
p {
  color: green;
}
```
Multiple HTML element:
```css
p, li {
    color: green;
}
```
## Styling with class
```html
<ul>
  <li>Item one</li>
  <li class="special">Item two</li>
  <li>Item <em>three</em></li>
</ul>
```
```css
.special {
  color: orange;
  font-weight: bold;
}
```

# Advanced selectors
## Selecting with state
[Styling with state](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/Getting_started#styling_things_based_on_state)
```css
a:link {
  color: pink;
}

a:visited {
  color: green;
}
```

## Combining selectors and combinators
```css
body h1 + p .special {
  color: yellow;
  background-color: black;
  padding: 5px;
}
```

# Values
- px
- em, rem
- %
- vh, vw
- calc()
- var()

# SCSS
[SCSS Basic](https://sass-lang.com/guide)