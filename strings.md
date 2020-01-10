# Strings

Strings are used for holding text values.

* There are single quotes, double quotes and back ticks:

```javascript
const name = 'orla';
const name = "orla";
const name = `orla`;
```

* Single quotes and double quotes are the same.
* Either can be used, but if you want to use ' or " in the text, you need to escape the text using a foreward slash:

```javascript
const name = 'orla\'s brain is "nice"';
const name = "orla's brain is \"nice\"";
```

* Using back ticks eliminates the need to escape the text

* Concatination is when two strings are combined into one
* Interpolation is when a variable is put inside a string

```javascript
const hello = "Hello my name is " + name + ". Hey!"; //combining strings and variables
```

* **Opinion** - using back ticks is more beneficial, and template literals can be used

```javascript
const hello = `hi my name is ${name} and I am ${age} years old`;
```

* It is also useful for creating html
```javascript
const html = `
<h1>${name}</h1>;
`
```
