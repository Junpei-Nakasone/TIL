# indexOf()

The `indexOf()` method returns the first index of a specified value(receive as argument).

Below example finds first index of "blue":
```js
const color = ["red", "blue", "green"];
let index = color.indexOf("blue"); // 1
```

You can specified offset with second argument. Below example starts at index 3:
```js
const color = ["red", "blue", "green","red"];
let index = color.indexOf("red", 3); // 4
```

The `indexOf()` method returns `-1` if the value is not found.
