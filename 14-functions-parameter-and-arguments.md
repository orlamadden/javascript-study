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

* Default values can be set incase someone forgets to pass an argument

```javascript
function yell(name = 'Silly Goose') {
    return `HEY ${name.toUpperCase()};
}

yell('Orla') // returns HEY ORLA
yell() // returns HEY SILLY GOOSE
```

* If we wanted to pass only the billAmount and tipRate, but not the taxRate so it will use its default value, we need to pass the taxRate arguement as undefined

```javascript
function calculateBill(billAmount, taxRate = 0.23, tipRate = 0.2) {
  const total = billAmount + billAmount * taxRate + billAmount * tipRate;
  return total;
}

console.log(calculateBill(100, undefined, 0.4)); // defaults to set taxRate as above in the function parameters
```