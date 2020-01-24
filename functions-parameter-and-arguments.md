# Parameters and Arguments

* Parameters are passed into a function, they are placeholder variables
* Arguements are values that are passed through the function
* When the function is defined, you can pass the arguments/value through the function

```javascript
function calculateBill(billAmount, taxRate) // parameters (placeholders)

calculateBill(100, 0.34) // arguments (values) passed through when calling the function
```
* A function can take values directly, as a value, and as an expression

```javascript
calculateBill(100, 0.23) // direct
calculateBill(myBill, myTax) // variables
calculateBill(20 + 20 + 3 + 4, 0.23) // expressions
```

* Functions can also be passed through a function

```javascript
function doctorize(name) {
  return `Dr. ${name}`;
}

console.log(doctorize('Orla')); // returns Dr. Orla

function yell(name) {
  return `HEY ${name.toUpperCase()}`;
}

console.log(yell('orla')); // returns HEY ORLA

console.log(yell(doctorize('orla'))); // returns HEY DR. ORLA
```