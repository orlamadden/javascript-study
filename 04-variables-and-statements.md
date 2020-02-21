# Variables

A variable is a container for storing values:

```javascript
let name = 'orla'; // orla is our value of the name variable

```

There are 3 ways to declare a variable:

```javascript
var name = 'orla'; 
let name = 'orla';
const name = 'orla';
```

* ```var``` and ```let``` values can be updated, ```const``` can not be updated
* ```var``` or ```let``` just need to be declared once, and then the values can be updated in the future, e.g:

```javascript
let age = 29;
age = 31;
```

* If we try to update a ```const``` variable, it throws an error, e.g:

```javascript
const age = 29;
age = 31; // will result in an error in the console
```
* Redeclaring a variable is considered bad practice like so:
```javascript
var name = 'orla';
var name = 'orla borla';
```

* It is also considered bad practice to declare a variable like:
```javascript
name = 'orla'; // a variable without let, var or const
```
* This will work but may cause bugs/issues down the line
* In strict mode, the variable needs to be defined or the code will not work:
```javascript 
name = 'orla'; // bad practice
console.log(name); // orla (no error) 
  
'use strict';
name = 'orla'; // error: name is not defined
  ```