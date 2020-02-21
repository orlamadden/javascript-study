# Functions - Custom

* Functions are created or defined, and then they are later called

```javascript
// defining the function - setting it up
function calculateBill() {
// function body
    console.log('calculating...');
    const total = 100 * 1.12;
    return total; // returns 111.9999999999999
}

calculateBill(); // running or calling the function
```

* Variables created inside a variable are only accessible in that function. This is called scoping

* The variable created inside a function is a temporary variable. After the function is finished running, the variable is cleaned up or 'garbage-collected'

* Capturing the returned value from a function inside a variable

```javascript
const billTotal = calculateBill();
```