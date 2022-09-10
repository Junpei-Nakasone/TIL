# await

`await` is only valid in async functions.
`await` operator is used to wait for `Promise`.

### Syntax
return_value = await expression

[expression]
Any value to wait for or A `Promise`.


```javascript
const getUsers = async () => {
  const URL = 'https://jsonplaceholder.typicode.com/users'

  res = await fetch(URL);

  res = await res.json()
  console.log(res) // userdata
}
```
