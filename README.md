# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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
## Desktop View 
![alt text](https://github.com/Gagana999/Create-Social-Links-Profile-Using-HTML-CSS/blob/main/design/destkop-design.jpg)

## Mobile View
![alt text](https://github.com/Gagana999/Create-Social-Links-Profile-Using-HTML-CSS/blob/main/design/mobile-design.jpg)

### Links

- Live Site URL: [Click here to visit the site](https://social-links-by-gagana.netlify.app)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Animations
- Desktop-first workflow

### What I learned

I Learnded things about that make responsive webiste and how to upload it to github. And how to upload it to online that anyone can see

To see how you can add code snippets, see below:

## HTML

```html
  <main>
    <div class="wrapper">
      <div class="social-links-card">
        <img src="assets/images/avatar-jessica.jpeg" alt="this is a image of a girl">
        <h1 class="name">Jessica Randall</h1>
        <p class="loaction">London, United Kingdom</p>
        <p class="description">"Front-end developer and avid reader."</p>
        <ul>
          <li><a href="#">GitHub</a></li>
          <li><a href="#">Frontend Mentor</a></li>
          <li><a href="#">LinkedIn</a></li>
          <li><a href="#">Twitter</a></li>
          <li><a href="#">Instagram</a></li>
        </ul>
      </div>
    </div>
  </main>
```

## CSS
```css
:root{
     --clr-accent-green: hsl(75, 94%, 57%);
     --clr-white: hsl(0, 0%, 100%);
     --clr-grey: hsl(0, 0%, 20%);
     --clr-dark-gray: hsl(0, 0%, 12%);
     --clr-black: hsl(0, 0%, 8%);

     --ff-base: 'Inter', sans-serif;

     --fw-light: 400;
     --fw-regular: 600;
     --fw-bold: 700;
}

/* ---------------------------------CSS RESET--------------------------------- */

/*
1. Use a more-intuitive box-sizing model.
*/
*, *::before, *::after {
     box-sizing: border-box;
}
/*
2. Remove default margin
*/
* {
     margin: 0;
}
/*
Typographic tweaks!
3. Add accessible line-height
4. Improve text rendering
*/
body {
     line-height: 1.5;
     -webkit-font-smoothing: antialiased;
}
/*
5. Improve media defaults
*/
img, picture, video, canvas, svg {
     display: block;
     max-width: 100%;
}
/*
6. Remove built-in form typography styles
*/
input, button, textarea, select {
     font: inherit;
}
/*
7. Avoid text overflows
*/
p, h1, h2, h3, h4, h5, h6 {
     overflow-wrap: break-word;
}
/*
8. Create a root stacking context
*/
#root, #__next {
     isolation: isolate;
}


/* Cutsome CSS */

body{
     color: var(--clr-white);
     background-color: var(--clr-black);
     font-family: var(--ff-base);
}
.wrapper{
     width: 100%;
     min-height: 100vh;
     display: flex;
     align-items: center;
     justify-content: center;
}
.social-links-card{
     --padding: 2rem;
     width: 25rem;
     background-color: var(--clr-dark-gray);
     padding: var(--padding);
     border-radius: 1rem;
     display: flex;
     align-items: center;
     justify-content: center;
     flex-direction: column;
}
.social-links-card img{
     border-radius: 100%;
     width: 5rem;
     margin-block: 2rem;
}
.name{
     font-weight: var(--fw-regular);
     font-size: 1.6rem;
}
.loaction{
     color: var(--clr-accent-green);
     font-size: 0.875rem;
     font-weight: var(--fw-bold);
}
.description{
     font-size: 0.875rem;
     font-weight: var(--fw-light);
     padding: var(--padding);
     text-align: center;
}
ul{
     width: 100%;
     padding: 0;
}

ul li a{
     text-decoration: none;
     color: var(--clr-white);
     font-size: 0.875rem;
     font-weight: var(--fw-bold);
     text-align: center;
     transition: color 0.7s linear;
}

ul li{
     text-align: center;
     width: 90%;
     list-style: none;
     text-decoration: none;
     background-color: var(--clr-grey);
     padding: 0.675rem 2rem;
     margin: 1rem;
     border-radius: 0.575rem;
     cursor: pointer;
     transition: background 0.7s linear;
}

ul li:is(:hover, :active){
     background-color: var(--clr-accent-green);
}
ul li:is(:hover, :active) a{
     color: var(--clr-black);
}

@media(max-width: 420px){
     .social-links-card{
          --padding: 0.675rem;
          margin: 1rem;
     }
     ul li{
          padding: 0.975rem 2rem;
     }
}

}
```

## Author

- Name : NBG Rantharu
- Frontend Mentor - [@Gagana-Rantharu](https://www.frontendmentor.io/profile/Gagana999)
- Linkedin - [@Gagana-Rantharu](www.linkedin.com/in/gagana-rantharu-01a7092b5)
