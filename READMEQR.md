# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### Screenshot

![img of solution](<../../Qr code concept/Screen Shot 2024-01-12 at 16.17.10-fullpage.png>)

### Links

- Live Site URL: https://65a1d3d91e60c1605d297846--fanciful-maamoul-646f50.netlify.app/


## My process
So, I am a very new coder and wanted to try out Frontend Mentor. I decided to go with the QR code challenge, and after I had finished, I only optimized the card for desktop, so it was not responsive AT ALL because, as a newbie to web development, I find responsiveness one of the most challenging things to do.

After inspecting my design with dev tools and playing around a little bit, I found myself unhappy with how unresponsive it was. I decided to challenge myself further. The only way I know how to create responsive designs is with media queries, but I'll be honest; I'm not very good at it.

So, I decided to circumvent that problem by giving myself an even harder task, which was not using media queries, to take myself out of my comfort zone. By using (VW) for the content, I figured out I could get the card itself to scale with screen size. However, that left the image and font-size, which are not easily scaled with (VW). So, I had to get creative and use the CLAMP() function <!--Which I've never used before-->, which the browser takes the inputs() you give it <!--can be in any order such as (1REM 1VW 2REM) or (5VW 70% 100px)--> defined in 3 categories: 1st = MIN, 2nd = Preferred, 3rd = MAX. The browser chooses which to use based on the screen size. This makes for incredibly scalable content without the need for any media queries.

                                    <!--=============================================-->

### Built with

- Semantic HTML5 markup
- CSS
- Flexbox
- CSS Grid

### What I learned

Through the use of CLAMP() I learned that you can create scalable content without the need for media queries 
<!-- not that there's anything wrong with them but it's good to know that you don't NEED them for everything-->

```css
.content h1 {
  font-size: clamp(.3rem, 2.5vw, 4rem)
}



## Author

- Frontend Mentor - [@yljaksen](https://www.frontendmentor.io/profile/ljaksen)
