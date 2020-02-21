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
* Using the ```return``` keyword is an example of a 'explicit' return. It me ans we explicitly return a value
* 'Implicit' returns omit the use of the ```return``` keyword for concise code if you are creating quick one line snippets of code

```javascript
const inchToCM = (inches) => inches * 2.54;
```
* If there is one parameter, you can remove the parentheses from the function
```javascript
const inchToCM = inches => inches * 2.54;
```
* If there is two parameters, you must keep the parentheses
```javascript
const add = (a, b = 3) => a + b;
```
* A function containing an object can also be converted to an arrow function
```javascript
function makeABaby(first, last) {
  const baby = {
    name: `${first} ${last}`,
    age: 0
  };
  return baby;
}

// arrow function version 
const makeABaby = (first, last) => ({ name: `${first} ${last}`, age: 0});
```

* A callback function is a function that is passed through another function, and is called at a later point
```javascript
button.addEventListener('click', function() {
    console.log('Nice Job!!');
});
```

* Timer callbacks run after a specific amount of time - takes 2 paramenters, function and time
```javascript
setTimeout(function() {
    console.log('Done!');
}, 1000);
```