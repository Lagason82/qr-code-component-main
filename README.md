# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents ( I leave this here for my reference ).

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

I have just learned HTML CSS for about a month, a lot of things still giving me confusion, however only following tutorial on youtube will not take me anywhere, hence I try to challenge myself. bit by bit. hopefully with all the knowledge I gained in the future will bring food to my table. 

please do point out any part that is consider not a normal practice, so I can learn.

### Screenshot

![](./screenshot.jpg)


### Links

- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

it is really helpful to get a hand on the figma file, I was able to check the necessary details such as font size, letter spacing, etc

1. created a flexbox first -> center the flexbox in the middle of the page

### Built with

- Semantic HTML5 markup ( well I need to remind myself to properly insert these structure in the future.
- CSS custom properties
- Flexbox
- CSS Grid


### What I learned

1. centering the flexbox to the center of the page. did learn it on the lesson before,
2. once centered, I added class="card" and set to display Grid
3. added the QR code and paragraph.

How I structure the HTML

<body>
  <div class="container">

    <div class="card">
      <img class="qr-img" src="/images/image-qr-code.png" alt="QR">

      <P class="header-text">Improve your front-end skills by building projects</P>

      <P class="content-text">Scan the QR code to visit Frontend Mentor and take your coding skills to the next level</P>

    </div>
      <div class="attribution">
      Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
      Coded by <a href="#">Richard Lee</a>.
      </div>
  </div>
</body>

CSS below:
/* - Mobile: 375px
- Desktop: 1440px */


*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    font-size: 62.5%;
}

body {
    background-color:var(--slate-300-bdy)
}

:root {
--White: hsl(0, 0%, 100%);
--slate-300-bdy:hsl(212, 45%, 89%);
--slate-500-para: hsl(216, 15%, 48%);
--slate-900-para:hsl(218, 44%, 22%);

/* paragraph font size */
--para: 1.5rem;

}

.attribution { font-size: 11px; text-align: center; }
.attribution a { color: hsl(228, 45%, 44%); }

/* body color to set here after this */

.container {
    display: flex;
    flex-direction: column;
    max-width: 1440px;
    margin: 0 auto;
    justify-content: center;
    align-items: center;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
}

.card {
    background-color:var(--White);
    display: grid;
    grid-template-columns: 1fr;
    width: 320px;
    align-items: center;
    justify-items: center;
    border-radius: 2rem;
    text-align: center;
    margin-bottom: 2rem;
    
}

.qr-img {
    width: 28.8rem;
    height: 28.8rem;
    border-radius: 2rem;
    margin: 1.6rem 1.6rem 2.4rem; 
}

.header-text {
    font-size: 2.2rem;
    font-weight: 700;
    color: var(--slate-900-para);
    padding-left: 1.6rem;
    padding-right: 1.6rem;
    line-height: 120%;
    padding-bottom: 1.6rem;
}

.content-text {
    font-size: 1.5rem;
    font-weight: 400;
    color: var(--slate-500-para);
    padding-left: 1.6rem;
    padding-right: 1.6rem;
    letter-spacing: 0.2px;
    line-height: 140%;
    padding-bottom: 4rem;
}


### Continued development

familiarise with how things work ( how flexbox, grid behave, how positioning work). then I will focusing more on e-commerce front-end build.


### Useful resources

MDN Website is really helping me a lot


## Author

- Website - I don't have one currently. still learning, only posting on github
- Frontend Mentor - [@Lagason82](https://www.frontendmentor.io/profile/Lagason82)


## Acknowledgments

frontendmentor was the first website I tried to do Challenge on, as it is really recommended by lot of people.


