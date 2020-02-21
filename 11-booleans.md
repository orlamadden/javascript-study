# Boolean

* A boolean is true or false, it's on or off

```javascript
let isDrawing = false; 
```
* Usely used for logic in if statements
* Can be manually set or calculated

```javascript
const age = 21; // sets the age to 21
const ofAge = age > 25; // sets variable to calculate if age is greater than 25
console.log(ofAge); // returns false as age is NOT greater than 25
```

* One equals is used to set a variable
```javascript
let age = 99;
```

* Always use triple equals ```===```, double equals ```==``` is sometimes considered bad practice unless its a use case scenario

```javascript
age === 99; // returns true
```

* Triple equals will always check for value and type, double equals only checks value
```javascript
10 === 10; // true, both have the same type and value
'10' == 10; // returns true, as the value is the same
'10' === 10; // returns false, as the value and type are not the same
```