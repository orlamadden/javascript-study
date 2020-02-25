# Scope

* Scope allows you to determine where are your funcitons and variables available to you

### Global variable
* A variable that can be accessed anywhere - inside and outside of a function
* ```var``` variables are attached to the window, they are globally scoped. ```const``` and ```let``` are not attached to the window.

### Function scope
* When variables are created inside a funtion, they are only available inside that function
```javascript
const age = 100;

function go() {
  const hair = 'blonde';
}

console.log(age); // logs 100
console.log(hair); // logs undefined
```
* You can name variables the same thing, once they are not in the same scope. This hinders accessing variables

### Variable Scoping

* let, var and const are all scoped differently
* var is function scoped, let and const are block scoped
* Curly brackets { } are blocks, or gates, that keep variables in
* From outside the blocks, you are not allowed to access whats inside the blocks

```javascript
if (1 === 1) {
  // const cool = true; // can't be accessed
  // let cool = true; // can't be accessed
  // var cool = true; // can be accessed 
}

console.log(cool);
```

