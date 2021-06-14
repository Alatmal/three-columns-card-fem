# Frontend Mentor - 3-column preview card component solution

This is a solution to the [3-column preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/3column-preview-card-component-pH92eAR2-). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned
For this challenge I applied flexbox where I thought it would be more efficient. Using the child selector for all the child elements in order achieve an even distribution for each segment. The flex-basis property was a great approach to make it. I had some troubles with the buttons to make them equal in height inside each car segment, although my solution was changing the position of each button to absolute and relative to their parent, now I consider that by justifying the content (h2, p and buttons) to space-between would have made things more easier and efficient. 

My flex-basis code: 

```css
.container{
    margin: 120px 60px 200px 60px;
    display: flex;
    flex-direction: column;
}

.container > *{
    flex-basis: 100%;
}
```

My not so efficient solution for button position in media query for the desktop version:

```html
<div class="car-type luxury">
      <div class="icon">
        <img src="images/icon-luxury.svg" alt="sedan icon">
      </div>
      <h2>Luxury</h2>
      <p>
      Cruise in the best car brands without the bloated prices. Enjoy the enhanced comfort of a luxury 
      rental and arrive in style.
      </p>
      <button type="submit">Learn More</button>
    </div>
```
```css
 .car-type{
        position: relative;
        padding: 40px 55px 0 35px;
    }

    .car-type button{
        width: 140px;
        position: absolute;
        bottom: 20px;
    }
```

### Continued development

I woul like to keep improving my flex and grid skills. My understanding in mode box size of html will be critical to make that happen. 


## Author

- Frontend Mentor - [@Alatmal](https://www.frontendmentor.io/profile/Alatmal)

