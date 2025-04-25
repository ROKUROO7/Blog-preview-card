# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

- Screenshot from a Desktop/Tablet

![Desktop](Desktop.jpeg)

- Screenshot from a Smartphone

![smartphone](smartphone.jpeg)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [https://rokuroo7.github.io/Blog-preview-card/](https://rokuroo7.github.io/Blog-preview-card/)

## My process

### Built with

- Semantic HTML5 markup
- CSS pseudo-class (no class="" or id="" was used)
- Flexbox
- Media-quary

### What I learned

while working on this project i noticed that the desktop preview used the default svg file and the smartphone preview used a cropped svg file.

so first i created another copy of the default svg file and modified that svg files width and viewbox.

Then i searched for a solution where i can use multiple images as src and let the browser choose an image based on the device width. 

At MDN i looked at an article named responsive images and found the solution under art-direction. 

I used picture tag to load two different svg files based on the device width.

```html
  <picture>
    <source media="(min-width: 401px)" srcset="/blog-preview-card-main/assets/images/illustration-article.svg">
    <source media="(max-width: 400px)" srcset="/blog-preview-card-main/assets/images/illustration-article-smartphone.svg">
    <img src="/blog-preview-card-main/assets/images/illustration-article.svg">
  </picture>
```

If anyone want to know more about this, I'd recommend checking out [The Responsive images](https://developer.mozilla.org/en-US/docs/Web/HTML/Guides/Responsive_images) to learn more.

## Author

- Frontend Mentor - [@ROKUROO7](https://www.frontendmentor.io/profile/ROKUROO7)
