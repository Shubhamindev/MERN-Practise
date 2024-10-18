CSS Selectors Reference

live preview
https://gleeful-sunshine-6be1bd.netlify.app/



CSS Selectors Reference
This repository provides a basic reference for various CSS selectors and their usage. Below are examples demonstrating different CSS selectors with corresponding styling.

Table of Contents
Basic Selectors
Class and ID Selectors
Attribute Selectors
Pseudo-Classes
Pseudo-Elements
Combinators
Colors and Styling
Basic Selectors
html
Copy code
<p>This paragraph is styled using a basic selector.</p>
css
Copy code
p {
    color: blue;
    font-size: 18px;
}
Class and ID Selectors
html
Copy code
<h1 class="highlight">This is a heading with class "highlight".</h1>
<p id="unique">This paragraph has an ID "unique".</p>
css
Copy code
.highlight {
    color: darkgreen;
    font-weight: bold;
}

#unique {
    color: purple;
    font-size: 20px;
}
Attribute Selectors
html
Copy code
<a href="https://example.com" target="_blank">This is a link to Example</a>
<input type="text" placeholder="Enter your name">
css
Copy code
a[target="_blank"] {
    color: red;
    text-decoration: underline;
}

input[type="text"] {
    border: 2px solid gray;
    background-color: lightyellow;
}
Pseudo-Classes
html
Copy code
<a href="#" class="btn">Hover over this link</a>
css
Copy code
/* Change color on hover */
.btn:hover {
    background-color: lightblue;
    color: white;
}

/* Change background when a link is visited */
a:visited {
    color: purple;
}
Pseudo-Elements
html
Copy code
<p>This paragraph has a styled first letter.</p>
css
Copy code
/* Style the first letter */
p::first-letter {
    font-size: 2em;
    color: red;
    font-weight: bold;
}
Combinators
html
Copy code
<div class="container">
    <h2>Sibling Heading</h2>
    <p>Paragraph next to the heading</p>
    <span>Child span element</span>
</div>
css
Copy code
/* Adjacent sibling combinator */
h2 + p {
    color: orange;
}

/* Child combinator */
.container > span {
    background-color: lightgreen;
}
Colors and Styling
Below are some examples of how to set colors, fonts, and other styles.

html
Copy code
<p class="colored">This paragraph is styled with multiple properties.</p>
css
Copy code
.colored {
    color: #3498db; /* Hex color */
    background-color: rgba(255, 99, 71, 0.5); /* RGBA color */
    font-family: Arial, sans-serif;
    text-align: center;
    text-transform: uppercase;
    line-height: 1.5;
    letter-spacing: 2px;
}
Media Queries
html
Copy code
<p class="responsive">Resize the window to see the effect.</p>
css
Copy code
/* Media query for screens larger than 600px */
@media (min-width: 600px) {
    .responsive {
        color: green;
        font-size: 24px;
    }
}
Animation
html
Copy code
<div class="box">Animated Box</div>
css
Copy code
@keyframes move {
    0% { transform: translateX(0); }
    50% { transform: translateX(100px); }
    100% { transform: translateX(0); }
}

.box {
    width: 100px;
    height: 100px;
    background-color: lightcoral;
    animation: move 3s infinite;
}
