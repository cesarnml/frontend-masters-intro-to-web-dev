# Frontend Masters - Introduction to Web Development

<!-- TOC -->

- [Frontend Masters - Introduction to Web Development](#frontend-masters---introduction-to-web-development)
  - [Progress](#progress)
  - [Codepen Exercise Collection](#codepen-exercise-collection)
  - [HTML](#html)
  - [CSS](#css)

<!-- /TOC -->

## Progress

- [X] *HTML* [2018-05-25]
- [ ] CSS
- [ ] JavaScript
- [ ] JQuery
- [ ] AJAX
- [ ] Command Line
- [ ] Node.js

## Codepen Exercise Collection

- [CodePen Exercise Collection](https://codepen.io/collection/DykjPp/)

## HTML

- `<html>` Encompasses your entire document.
- `<meta>` Where meta data lives. Never displayed.
- `<body>` Display content goes here.
- Common HTML tags: `<h1>` ... `<h6>`, `<p>`, `<div>`, `<ul>`, `<ol>`, `<li>`, `<strong>`, `<em>`, `<span>`
- HTML tags/elements can be assigned _attributes_
- The _class_ attribute is used to identity the tag semantically
- The _id_ attribute is similar, but should be unique, whereas the _class_ attribute is meant to be on reusable tags.

```html
<tag attribute='value' class='className'>Content</tag>
```

- Don't use 'presentational names' for _class_ or _id_ names. Use names that say 'what something is', not where it is on your page or what it looks like.

## CSS

- Because I always forgot:

```html
box-styling: content-box // never use

* {
box-styling: border-box // yass!
}
```

- Hahaha. 'FlexBox is kinda hard.' (2014)
- Checkout **normalize.css**
- `clear fix` Look up later. If maintaining old code.
- `overflow: hidden` to consider if tackling the great collapse.