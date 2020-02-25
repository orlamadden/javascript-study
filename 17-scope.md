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