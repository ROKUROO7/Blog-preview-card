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
![/Desktop.jpeg](./Desktop-view.jpeg)

- Screenshot from a Smartphone
![/smartphone.jpeg](./Smartphone-view.jpeg)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS pseudo-class (no class="" or id="" was used)
- Flexbox
- Media-quary

### What I learned

while working on this challenge i noticed the desktop view used the full width for the svg file  and the smartphone view used a lower width with cropped svg file. so i looked for responsive images in MDN and found two soultions.one with the img srcset tag and the other one using picture source tag.

In this Challenge I used picture source tags.

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
