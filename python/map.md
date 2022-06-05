# map() function


### syntax
map(function, iterables)

- function(required): this is the function to execute for each item.

- iterables(required): collection of object.

```python
input_value = '1 2 3'
a, b, c = map(int, input_value.split())
print(a) # 1
print(b) # 2
print(c) # 3
```
