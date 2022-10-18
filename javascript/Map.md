# Array.from()

Array.from() creates an array from a string:
```js
Array.from("ABCD"); // ["A","B","C","D"]
```

`Array.from()` method returns an array from any object with a length property and/or any iterable object.

You can not use Array.from() method if you create your own array because Array.from() is a static property of the JavaScript Array object.
```js
const x = ["A","B","C"];
x.from() // return undefined error
```

