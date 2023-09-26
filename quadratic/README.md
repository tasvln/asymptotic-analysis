# Quadratic

This is when the resource needed and the data being processed grows at a rate of n^2.

To my understanding, this is when you have a nested loop and the inner loop is dependent on the outer loop.

## Examples

```python
def quadratic(data):
  for i in range(0, len(data)): # (n - 1) + 1
    for j in range(0, len(data)): # (n - 1) + 1 = n (which loops n times, see below for calculation)
      return data[i] # 1(n) = n
```

##### First Loop

(n - 1) + 1 = n

##### Second Loop

(n - 1) + 1 = n 

multiplied by the first loop = n * n = n^2

Therefore, T(n) = n + n^2 + n

T(n) = 2n + n^2

T(n) = O(n^2)