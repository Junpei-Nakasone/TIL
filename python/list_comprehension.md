# List Comprehension

You can use list comprehension when you want to make new list based on the values of another existing list.

```python
example_list = ['1', '2','3']

new_list = [int(x) for x in example_list]

print(new_list) # [1, 2, 3]
```

You can also use basic for loop syntax but it would be longer than list comprehension.

```python
example_list = ['1', '2','3']
new_list = []
for i in range(len(example_list)):
  new_list.append(int(example_list[i]))
print(new_list) # [1, 2, 3]

```


```python
input2 = ['-8 7 6','-5 0 -1','3 6 -9']

test = [[int(x) for x in input2[i].split()] for i in range(n)]
print(test) # [[-8, 7, 6], [-5, 0, -1], [3, 6, -9]]
```
