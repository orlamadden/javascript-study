# Debugging Tools

1. Console Methods

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