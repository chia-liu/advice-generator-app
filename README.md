# Advice generator app
mobile-first workflow

# Frontend Mentor - Advice generator app solution

This is a solution to the [Advice generator app challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/advice-generator-app-QdUG-13db). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- 

### Screenshot

![](./design/active-states.jpg)


### Links

- Solution URL: [solution](https://github.com/chia-liu/advice-generator-app)
- Live Site URL: [live site](https://chia-liu.github.io/advice-generator-app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Mobile-first workflow
- JavaScript

### What I learned

fetch API 

```js 

const fetchAdvice = async() => {
    const res = await fetch("https://api.adviceslip.com/advice")
    const data = await res.json()

    console.log(data)

    document.getElementById("title").innerHTML = `Advice #${data.slip.id}`
    document.getElementById("text").innerHTML = `"${data.slip.advice}"`
}

fetchAdvice()

```


## Author

- Frontend Mentor - [@chia-liu](https://www.frontendmentor.io/profile/chia-liu)
- Github - [@chia-liu](https://github.com/chia-liu)

