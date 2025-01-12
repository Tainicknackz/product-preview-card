# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![Desktop image](./screenshots/desktop-design.jpg)
![Mobile image](./screenshots/mobile-design.jpg)

### Links

- Solution URL: [github.com/Tainicknackz/product-preview-card](https://github.com/Tainicknackz/product-preview-card)
- Live Site URL: [capable-sopapillas-2e96af](https://app.netlify.com/sites/capable-sopapillas-2e96af/deploys/67836906986e40bd644d90d8)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Flexbox
- Mobile-first workflow

### What I learned

_Flex-box_ and _Media Queries_ were clear to me. How to keep columns responsive and scalable. **As shown below:-**

```html
<!-- Parent container -->
<div class="perfume-card__content">
  <!-- Image Container -->
  <div class="perfume-card__img-ctn"></div>
  <!-- Description Container -->
  <div class="perfume-card__desc"></div>
</div>
```

```css
@media (min-width: 1440px) {
  /* Card-content */
  .perfume-card__content {
    display: flex;
    flex-direction: row;
    background-color: hsl(0, 0%, 100%);
    border-radius: 13px;
    overflow: hidden;
  }

  /* Image-container */
  .perfume-card__img-ctn {
    display: flex;
    flex: 1 1 50%;
    justify-content: center;
    align-items: center;
  }

  /* Description-container */
  .perfume-card__desc {
    display: flex;
    flex-direction: column;
    flex: 1 1 50%;
    margin: 0 auto;
    padding: 2.5rem;
  }
}

@media (max-width: 375px) {
  /* Card-content */
  .perfume-card__content {
    display: flex;
    flex-direction: column;
    border-radius: 13px;
    background-color: hsl(0, 0%, 100%);
    overflow: hidden;
  }

  /* Image-container */
  .perfume-card__img-ctn {
    display: flex;
    flex: 1;
    align-items: center;
    justify-content: center;
    max-height: 265px;
  }

  /* Description-container */
  .perfume-card__desc {
    display: flex;
    flex-direction: column;
    flex: 1;
    margin: 0 auto;
    padding: 1em;
  }
}
```

- Website - [capable-sopapillas-2e96af](https://capable-sopapillas-2e96af.netlify.app)
- Frontend Mentor - [@Tainicknackz](https://www.frontendmentor.io/profile/Tainicknackz)
- GitHub - [@Tainicknackz](https://www.github.com/Tainicknackz)
