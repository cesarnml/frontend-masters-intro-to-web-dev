# Frontend Masters - Introduction to Web Development (2014 - bit out-of-date)

<!-- TOC -->

- [Frontend Masters - Introduction to Web Development (2014 - bit out-of-date)](#frontend-masters---introduction-to-web-development-2014---bit-out-of-date)
  - [Progress](#progress)
  - [Codepen Exercise Collection](#codepen-exercise-collection)
  - [HTML](#html)
  - [CSS](#css)
    - [JavaScript](#javascript)
    - [jQuery](#jquery)
    - [AJAX](#ajax)
    - [Command Line (More Like Basic Git/GitHub)](#command-line-more-like-basic-gitgithub)

<!-- /TOC -->

## Progress

- [X] *HTML* [2018-05-25]
- [X] *CSS* [2018-05-25]
- [X] *JavaScript* [2018-05-26]
- [X] *JQuery* [2018-05-26]
- [X] *AJAX* [2018-05-26]
- [X] *Command Line* [2018-05-27]
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
- Neat hack near the end of the video about vertically-center text above an image. All the hacks seem out of date tho ...

### JavaScript

- Very basic introduction to JS. I didn't learn anything worth noting. It was a bit annoying when that the instructor kept refering to arrays as 'lists'.
- The instructors butchered the _context_ of _this_. Here is the code they were trying to accomplish.

```javascript
const car = {
  type: 'Corolla',
  sayType: function() {
    return this.type
  }
}

const luxCar = {
  type: 'Lexus'
}

let myCar = car.sayType

myCar = myCar.bind(luxCar)

console.log(myCar()) //  Lexus

console.log(car.sayType()) // Corolla
```

### jQuery

- `$('.class or #id').method()` jQuery in a nutshell
- Again, the course is very basic. There wasn't much of note.

### AJAX

- Asynchronous JavaScript and XML
- Code Sample:

```javascript
$('.btn').click(function() {
  $('.text').text('Loading...')
  $.ajax({
    type: 'GET',
    url: 'https://www.reddit.com/r/aww/search.json?q=puppy&restrict_sr=true',
    success: function(data) {
      $('.text').text('')
      const dogArr = data.data.children
      for (let i = 0; i < dogArr.length; i++) {
        $('.text').append(`<img src=${dogArr[i].data.thumbnail}>`)
      }
    }
  })
})
```

- Basic intro. Not much of note.

### Command Line (More Like Basic Git/GitHub)

- Nothing worth noting. Basic Git/GitHub workflow
- I regret spending 10 hours on this course. It was far below the level of Lambda School's curriculum.
