# Numbers

* There is only one type of number in Javascript, regardless if it is an integer or float:

```Javascript
const numOne = 34; // integer
const numTwo = 3.4; // float - with decimal point

```

* The ```typeof``` operator returns the data type of the operand:
```Javascript
const name = 'orla'; // variable with string
const age = 400; // variable with number

typeof name; // will return 'string'
typeof age; // will return 'number'
```

* Adding a number and string will concatinate the data:

```Javascript
1 + '1'
'11'
```

* Javascript has Math helper methods
```Javascript
Math.round(50.3); // rounds to nearest whole number - 50
Math.floor(50.3); // rounds down to nearest whole number - 50
Math.ceil(50.3); // rounds up to nearest whole number - 51
Math.random(); // returns random number between 0 and 1
```

* Modulus returns the division remainder of numbers:

```Javascript
/* We want to divide an equal amount of Pokemon to trainers
and return the remainder to Professor Oak
*/
const pokemon = 27; // 27 Pokemon available
const trainers = 4; //
const eachTrianerGets = Math.floor(pokemon / trainers); // returns 6
const profOak = pokemon % trainers; // returns 3
```

* There is a max on how far the computer can count with numbers, Infinity and minus Infinity are true numbers:

```Javascript
10 ** 2; // 10 to the power of 2 returns 100
10 ** 25; // 10 to the power of 25 returns Infinity
```

* ```NaN``` is a number

