# Frontend Mentor – QR Code Component Solution

This is my solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

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

### Screenshot

![](./screenshot.png)

### Links

- **Solution URL:** https://github.com/tomasgarbarino/qr-code-component  
- **Live Site URL:** https://tomasgarbarino.github.io/qr-code-component/  

## My process

### Built with

- Semantic HTML5  
- CSS3  
- CSS custom properties  
- Flexbox  
- Mobile-first responsive design  

### What I learned

- **Centering with Flexbox vs Absolute Positioning**  
  I switched the card centering from `position: absolute` + `transform` to Flexbox on the body, which simplifies the layout and makes it inherently responsive:
  ```css
  body {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
  }
  ```

- **Responsive images**  
  Making the QR code image adapt to container width while preserving aspect ratio:
  ```css
  .qr-code {
    width: 100%;
    max-width: 288px;
    height: auto;
    border-radius: 0.625rem;
    display: block;
    margin: 0 auto;
  }
  ```

- **CSS custom properties**  
  Centralized colors, spacing, and typography variables for consistency and easier theming:
  ```css
  :root {
    --bg-page: #D5E1EF;
    --bg-card: #FFFFFF;
    --clr-text: #1F2937;
    --clr-sub: #6B7280;
    --radius: 1.25rem;
  }
  ```

## Continued development

- Practice CSS Grid for more complex layouts.  
- Add subtle hover/focus animations to improve interactivity.  
- Explore ARIA roles and additional semantic elements for better accessibility.  

## Useful resources

- CSS Custom Properties on MDN – comprehensive guide to CSS variables.  
- A Complete Guide to Flexbox – patterns and use cases for Flexbox layouts.  
- Frontend Mentor challenge description – original challenge specification.  

## Author

Tomas Garbarino

- GitHub: @tomasgarbarino  
- Frontend Mentor: @tomasgarbarino  

## Acknowledgments

- Thanks to Frontend Mentor for providing the challenge.  
- MDN Web Docs for detailed HTML & CSS documentation.  
- CSS-Tricks community for layout and accessibility tips.