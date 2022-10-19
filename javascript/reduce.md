# reduce()

`reduce()` method executes a reducer function for array element.

`reduce()` methods returns a single value(the function's accumulated result) and does not change the original array.

## Syntax
`array.reduce(function(total, currentValue), initialValue)`

|Parameter|Description|
---|---
|Reducer function()|A function which runs for each element in the array. Required.|

Reducer function parameters:

|Parameter|Description|
---|---
|total|The initial Value or previously returned value of the reducer function. Required.|
|current value|The value of current element. Required.|
|current index|The index of the current element. Optional.|
|arr|The array the current element belongs to. Optional.|
