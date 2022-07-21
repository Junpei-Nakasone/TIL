# Arrow function

You can make function syntax shorter by using arrow function.

Without arrow function.
```JavaScript
hello = function() {
  return "this is example";
}
```

With arrow function.
```JavaScript
hello = () => {
  return "this is example";
}
```

You can also remove the bracket and the `return` keyword if the function has only one statement and statement returns a value.

```JavaScript
hello = () => "this is example";
```
