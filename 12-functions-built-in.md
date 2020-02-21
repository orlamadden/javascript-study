# Functions (Built In)

* Functions allow us to group instructions, they are groups of statements

* Functions take in data called **arguments**

```javascript
Math.max(); // built in function
Math.max(10, 12); // 10 and 12 are the arguments passed through
12 // returns 12

parseFloat('20.57849'); //parses a string and returns 
// a floating point number
parseInt ('20.4566'); // parses a string and returns an integer
Date.now(); // returns the date in milliseconds
```

* Some functions work with the DOM

```javascript
const p = document.querySelector('p'); // selects first p tag in html document
console.log(p); // logs the selected p tag to the console
```

* [Mozilla Developer Network (MDN)](https://developer.mozilla.org/en-US/docs/Web/JavaScript) is a fantastic resource for all things Javascript

```javascript
scrollTo (0, 300); // scrolls to x, y position on screen
scrollTo ({top: 400, left: 0, behavior: 'smooth'}); // scroll options, scrolls to position on screen smoothly
```