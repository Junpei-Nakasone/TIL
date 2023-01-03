# Python Lambda
A lambda function is a samll anonymous function.
It can take any number of arguments, but can only have one expression.

### Syntax
```python
lambda arguments : expression
```

The expression is executed and the result is returned.

Add 3 to argument `x`, and return the result.
```python
y = lambda x : x + 10
print(y(10)) # 13
```

Lambda functions can take any number of arguments.

```python
x = lambda a, b : a + b
print(x(1,2)) # 3
```

The benefit of lambda is better shown when you use them as an anonymous function inside another function.

```python
def mylambda(c):
  return lambda a : a * n
```

Use above function definition to make a function that always doubles the number you send.

```python
def mylambda(n):
  return lambda a: a * n

doubler = mylambda(2)

print(doubler(11)) # 22

tripler = mylambda(3)

print(tripler(11)) # 33
```

You can use lambda when you want to sort some list

items = []
