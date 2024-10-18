CSS Selectors Reference

live preview
https://gleeful-sunshine-6be1bd.netlify.app/



# CSS Selectors Reference

This repository provides a basic reference for various CSS selectors and their usage. Below are examples demonstrating different CSS selectors with corresponding styling.

## Table of Contents
1. [Basic Selectors](#basic-selectors)
2. [Class and ID Selectors](#class-and-id-selectors)
3. [Attribute Selectors](#attribute-selectors)
4. [Pseudo-Classes](#pseudo-classes)
5. [Pseudo-Elements](#pseudo-elements)
6. [Combinators](#combinators)
7. [Colors and Styling](#colors-and-styling)
8. [Media Queries](#media-queries)
9. [Animation](#animation)
10. [Additional Examples](#additional-examples)

## Basic Selectors

```html
<p>This paragraph is styled using a basic selector.</p>
p {
    color: blue;
    font-size: 18px;
}
```
Class and ID Selectors
```
<h1 class="highlight">This is a heading with class "highlight".</h1>
<p id="unique">This paragraph has an ID "unique".</p>
.highlight {
    color: darkgreen;
    font-weight: bold;
}

#unique {
    color: purple;
    font-size: 20px;
}

```

Attribute Selectors
```
<a href="https://example.com" target="_blank">This is a link to Example</a>
<input type="text" placeholder="Enter your name">
a[target="_blank"] {
    color: red;
    text-decoration: underline;
}

input[type="text"] {
    border: 2px solid gray;
    background-color: lightyellow;
}
```
Pseudo-Classes
```
<a href="#" class="btn">Hover over this link</a>
/* Change color on hover */
.btn:hover {
    background-color: lightblue;
    color: white;
}

/* Change background when a link is visited */
a:visited {
    color: purple;
}
```
Pseudo-Elements
```
<p>This paragraph has a styled first letter.</p>
/* Style the first letter */
p::first-letter {
    font-size: 2em;
    color: red;
    font-weight: bold;
}
```
Combinators
```
<div class="container">
    <h2>Sibling Heading</h2>
    <p>Paragraph next to the heading</p>
    <span>Child span element</span>
</div>
/* Adjacent sibling combinator */
h2 + p {
    color: orange;
}

/* Child combinator */
.container > span {
    background-color: lightgreen;
}
```
# Colors and Styling
## Colors and Styling

This section demonstrates how to apply different colors to elements using CSS. We cover text color, background color, borders, and gradients.

### Text Colors

You can set the text color using the `color` property. The value can be a named color, a hex code, an RGB value, or an HSL value.

#### CSS Example

```css
/* Using named colors */
h1 {
    color: darkblue;
}

/* Using hex codes */
h2 {
    color: #ff6347; /* Tomato color */
}

/* Using RGB */
p {
    color: rgb(60, 179, 113); /* Medium Sea Green */
}

/* Using HSL */
p.highlight {
    color: hsl(120, 100%, 25%); /* Dark Green */
}

```
```
<p class="colored">This paragraph is styled with multiple properties.</p>
.colored {
    color: #3498db; /* Hex color */
    background-color: rgba(255, 99, 71, 0.5); /* RGBA color */
    font-family: Arial, sans-serif;
    text-align: center;
    text-transform: uppercase;
    line-height: 1.5;
    letter-spacing: 2px;
}
```


