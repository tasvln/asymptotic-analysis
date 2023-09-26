# Constant Growth

When the resource does not grow, it is constant.

To my understanding, processing 1 piece of data = processing 1 million -> a billion -> a trillion pieces of data.

It means that no matter how much data you have, the time it takes to process it is the same.

## Examples

```python
def constant(data):
  return data # 1
```

T(n) = 1

T(n) = O(1)

```python
def constant(data):
  return data[0] # 1
```

T(n) = 1

T(n) = O(1)

```python
def constant(num):
  calc = ((number + 2) / 4 + 34 - (number * 2)) # 6 operations excluding the brackets
  return calc # 1
```

T(n) = 7

T(n) = O(1)

> number can be 1_000_000 but it will still take the same time to process it.
