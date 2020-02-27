# Hoisting

* Allows you to access functions and variables before they have been created
```javascript
sayHi(); // function declared BEFORE the function itself

function sayHi() {
  console.log('hey!'); // console logs hey!
}
```

* Only works with regular functions, not functions declared in variables