# Running and Loading Javascript

* We can run JS in the browser by accessing the Console in dev tools. Use CTRL+SHIFT+J to get to the console quickly.
* We can run JS in a standard HTML file by adding script tags in the ```<body>``` tag like below:
```javascript
<script>
var greeting = "Hello World";
alert(s);
</script>
```

* It is important to add the ```<script>``` just above the closing ```</body>``` tag as this will allow for access to HTML elements *above* the JS.
* Running JS before the HTML elements will not allow us to access HTML elements that come after it.
* We can run JS externally by linking to a JS ```src``` file using a relative path like below:
```javascript
<script src="./scripts.js"></script>
```