# Declaring Functions

* Functions can be stored as values in variables and other ways

* Declared with the **function keyword**
```javascript
function doctorize(firstName) {
  return `Dr.${firstName}`;
 }
```
_Note_: these function declarations are **hoisted**, meaning JS takes it up to the top of the file and is made available befor it is declared

* **Anonymous function** - a function without a name - valid in use cases
* Used in callbacks and Immediately Invocked Function Expression (IIFE)

```javascript
// anonymous function
function (firstName) {
    return `Dr. ${firstName}`;
}
```

* Function expression - store a value in a variable

```javascript
const doctorize = function(firstName) {
    return `Dr. ${firstName};
}
```
_Note_: these function declarations are **not hoisted**, will give an error if called before it is declared

* Arrow functions - new addition to JS
* They are more concise
* Both examples give the same output, just one is a standard function and the other is an arrow function

```javascript
// keyword example
function inchToCM(inches) {
  const cm = inches * 2.54;
  return cm;
}

// arrow function example
const inchToCM = (inches) => {
    return inches * 2.54;
  };
```