# Debugging Tools

### Console Methods

* Console.log() - standard logging of data into the Console
* Console.error() - outputs an error to the Console
* Console.warn() - outputs a warning error to the Console
* Console.table() - outputs a table if you have a list of objects with the same property:
![image of a table](https://res.cloudinary.com/orla2020/image/upload/v1582095727/Javascript%20Course%20by%20Wes%20Bos/console-table_s9mtxo.png)

* Console.count() - shows how often a function is running
```Javascript
function doctorize(name) {
  console.count('Running this function');
  return `Dr. ${name}`;
}
```
![image of console.count function](https://res.cloudinary.com/orla2020/image/upload/v1582096408/Javascript%20Course%20by%20Wes%20Bos/console-count_dovky9.png)

* Console.group() - groups multiple logs within one log:
```Javascript
function doSomeStuff() {
  console.group('Do all this');
  console.log('HEllo world');
  console.count('this function');
  console.warn('warning');
  console.error('this is an error');
  console.groupEnd('Do all this');
}
```

* console.groupCollapsed() will automatically collapse data in the console, it will look nice and tidy:
```Javascript
const people = [
  { name: 'Orla', cool: true, country: 'Ireland' },
  { name: 'Dan', cool: true, country: 'Trinidad' },
  { name: 'Snickers', cool: false, country: 'Dog Country' },
];

// loops through the above
people.forEach((person, index) => {
  console.groupCollapsed(`${person.name}`);
  console.log(person.country);
  console.log(person.cool);
  console.log('Done');
  console.groupEnd(`${person.name}`);
});
``` 

### Stack Trace

* Allows us to find out what function called what function called what function....

```Javascript
function doctorize(name) {
  return `Dr. ${name}`;
}

function greet(name) {
  doesntExist(); // error
  return `Hello ${name}`;
}

function go() {
  const name = doctorize(greet('Wes'));
  console.log(name);
}
```
* If we run the function ```go()``` in the console, it will log an error as the function does not exist: 
![](https://res.cloudinary.com/orla2020/image/upload/v1582266272/Javascript%20Course%20by%20Wes%20Bos/console-error_dxray8.png)

* This method allows us to trace where the function is called so we can fix the bug.

### Grabbing Elements

* In Chrome Devtools, when you have an element selected in the 'Elements' tab, switch to console and type in ```$0```
* The 0 stands for the last element clicked
* It also works for ```$1``` which is second last element clicked, and ```$2``` which is third last element clicked
* $ and $$ are shorthand selectors

### Breakpoints

* The debugger keyword stops the code from executing and opens debugging in the console
```Javascript
people.forEach((person, index) => {
  debugger; // code stops here and debugging function opens
  console.groupCollapsed(`${person.name}`);
  console.log(person.country);
  console.log(person.cool);
  console.log('Done');
  console.groupEnd(`${person.name}`);
});
```

