# Frontend Mentor - Huddle landing page with curved sections solution

This is a solution to the [Huddle landing page with curved sections challenge on Frontend Mentor](https://www.frontendmentor.io/solutions/responsive-huddle-landing-page-using-css-grid-R1Dkw8az9u). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
	- [The challenge](#the-challenge)
	- [Links](#links)
- [My process](#my-process)
	- [Built with](#built-with)
	- [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Links

- [Solution URL](https://www.frontendmentor.io/solutions/responsive-huddle-landing-page-using-css-grid-R1Dkw8az9u)
- [Live Site URL](https://huddle-landing-page-challenge.netlify.app/)

## My process

### Built with

- HTML
- CSS
- JavaScript
- Flexbox
- CSS Grid
- Font Awesome for icons [Font Awesome](https://fontawesome.com/)

### What I learned

I thoroughly enjoyed this challenge 😅

This was my first time using CSS Grid, i've been wanting to experiment with it so learnt it whilst building this landing page. As well as getting stuck in with a responsive design from desktop to mobile was a great challenge.

Below is some of my CSS Grid code
```css
.grid {
		display: grid;
		grid-template-rows: 1fr;
		grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
		margin: 0 10%;
		column-gap: 5%;
	}

	.inner-grid {
		grid-column: 1;
		grid-row: 1;
		display: flex;
		flex-direction: column;
		justify-content: center;
		max-width: 80%;
		color: var(--VeryDarkCyan)
	}
```

Below was my first time validating an email input form by JavaScript
```js
function buttonValidation(email) {
		let element = document.getElementById("subscribe-form");
		let elementError = document.getElementById("email-error")
		let emailFormat = /^([A-Za-z0-9_\-\.])+\@([A-Za-z0-9_\-\.])+\.([A-Za-z]{2,4})$/;

if (email.value.match(emailFormat)) {
			return true;

		} else {
			element.classList.add("invalid");
			elementError.classList.add("email-error");
			document.subscribe.email.focus();
			return false;
		}
}
```

## Author

- Website - [Made by Willo](https://madebywillo.co.uk/)
- Frontend Mentor - [@Louise-Ann93](https://www.frontendmentor.io/profile/Louise-Ann93)
- Dev.to - [@louise-ann93](https://dev.to/louiseann93)

