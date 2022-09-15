# Use custom function in google spread sheet

By adding `@customfunction` tag in documentation comment, you can use your custom function which defined in Google Apps Script in Google Spread Sheet.


```JavaScript
/**
 * @customfunction
 */
function TESTFunction(value) {
  return 'this is test:' + value
}
```
