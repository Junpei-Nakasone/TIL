# 'str' object does not support item assignment

```python
example_input = ['##','##']
example_input[0][1] = '.'
# Exception has occurred: TypeError
#'str' object does not support item assignment
```

```python
# this code will work
example_input = [['#','#'],['#','#']]
example_input[0][1] = '.'
print(example_input) # [['#', '.'], ['#', '#']]
```
