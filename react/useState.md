# useState

`useState()` manages `state` in function component of React.
Initial value of `state` is first argument of `useSate`.

`useState()` Statement would be like bellow.

```js
const [state, function_updates_state] = useState(initialvalue);
```

Following code is simple `useState` usage from [react.js official docs](https://ja.reactjs.org/docs/hooks-overview.html
).

```js
import React, { useState } from 'react';

function Example() {
  // Declare a new state variable, which we'll call "count"
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```
