#### chain.from_iterable()

```python
nested_list = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
print(list(itertools.chain.from_iterable(nested_list))) # [1, 2, 3, 4, 5, 6, 7, 8, 9]
```

```python
nested_list_includes_duplicate = [[1, 2, 3], [4, 5, 6], [7, 8, 9], [1, 2, 3]]
print(list(set(itertools.chain.from_iterable(nested_list_includes_duplicate)))) # [1, 2, 3, 4, 5, 6, 7, 8, 9]
```

