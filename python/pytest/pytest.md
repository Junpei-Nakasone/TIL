`pytest` is test framework for python.
pytest required Python 3.7+ or PyPy3.

### How to write tests in pytest
You need
1. Define test as function
2. Validate it with assert statement

```python
def inc(x):
    return x + 1

def test_answer():
    assert inc(3) == 4
```
