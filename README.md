# Frontend Mentor - Fylo data storage component solution

This is a solution to the [Fylo data storage component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/fylo-data-storage-component-1dZPRbV5n). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### Screenshot

![](screenshots/desktop-preview.png)

### Links

- Solution URL: [https://github.com/miranlegin/fem-fylo-data-storage](https://github.com/miranlegin/fem-fylo-data-storage)
- Live Site URL: [https://frontend-mentor-challenge06.netlify.app/](https://frontend-mentor-challenge06.netlify.app/)

## My process

### Built with

- Icomoon fonts
- CSS animations/@keyframes
- Flexbox
- CSS Grid
- CSS only animated counter with CSS custom properties

### What I learned

That you can create animated CSS counters, examples in Section #Useful resources

```css
@property --num {
  syntax: '<integer>';
  initial-value: 0;
  inherits: false;
}

@keyframes counter {
  0% {
    --num: 0;
  }
  100% {
    --num: 815;
  }
}

.counter {
  ...
  counter-reset: num var(--num);
  animation: counter ...;

  &::after {
    content: counter(num);
  }
}
```

### Useful resources

- [@keyframes](https://developer.mozilla.org/en-US/docs/Web/CSS/@keyframes) - Documentation for creating animation in CSS.
- [Animating numbers with CSS only](https://css-tricks.com/animating-number-counters/) - With recent support for CSS.registerProperty and @property, we can animate CSS variables. The trick is to declare the CSS custom property as an integer; that way it can be interpolated (like within a transition) just like any other integer.
- [Cubic bezier functions](https://cubic-bezier.com/#.17,.67,.83,.67) - A better tool for cubic-bezier() easing
- [Easing functions](https://easings.net/) - Predefined easing functions .

## Author

- Frontend Mentor - [@miranlegin](https://www.frontendmentor.io/profile/miranlegin)
