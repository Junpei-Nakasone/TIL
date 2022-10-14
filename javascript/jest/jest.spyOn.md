# jest.spyOn(object, methodName)

Creates a mock function similar to `jest.fn()` but also tracks calls to `object[methodName]`.
Returns a Jest mock function.

Example code:
```js
const person = {
  walk() {
    return true;
  },
};

module.exports = person;
```

Example test:
```js
const person = require('./person');

afterEach(() => {
  // restore the spy created with spyOn
  jest.restoreAllMocks();
});

test('person walks', () => {
  const spy = jest.spyOn(person, 'walk');
  const isWalking = person.walk;

  expect(spy).toHaveBeenCalled();
  expect(isWalking).toBe(true);
});
```
