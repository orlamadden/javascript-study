# Closures

* The ability to access a parent level scope from a child scope even after the parent function has been closed or terminated

```javascript
function outer() {
  const outerVar = 'Hey I am the outer var!';
  
   function inner() {
    const innerVar = 'Hey I am an inner var!'
    console.log(innerVar)
    console.log(outerVar)

    
  }
  inner();
}
outer(); 
```
* The inner() function does a 'scope lookup' and see the outer function