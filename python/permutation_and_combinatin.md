## Permutation and Combination in Python

Python provides direct methods to find permutations and combinations of a sequence.
These methods are present in `itertools` package.

### Example

```python
from itertools import permutations

val = 123
val = str(val)
perm = permutations(val)

for i in list(perm):
    print(i)
# OUTPUT:
# ('1', '2', '3')
# ('1', '3', '2')
# ('2', '1', '3')
# ('2', '3', '1')
# ('3', '1', '2')
# ('3', '2', '1')
```

In above case, `val` should be cast to str because int is not iterable.

Without casting, an error occurs at permutations function which says `TypeError: 'int' object is not iterable`.
```python
from itertools import permutations

val = 123
# val = str(val)
perm = permutations(val) # TypeError: 'int' object is not iterable

for i in list(perm):
    print(i)

```

