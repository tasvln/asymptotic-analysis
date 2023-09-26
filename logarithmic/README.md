# Logarithmic

This is when the resource grows by one unit everytime the data is doubled.

To my understanding, the data being processed is halved in every iteration.

## Examples

The best example is a binary search.

in the first iteration, the data is halved, then halved again, and again, and again until the target is found. which results to our loop running 1 + log n times.

#### Best Case

```python
def binary_search(data, target):
  low = 0 # 1
  high = len(data) - 1 # 3

  while low <= high: # 1 (1 + log n)
    mid = (low + high) // 2 # 3(1 + log n)
    if target == data[mid]: # 1(1 + log n)
      return True # 1
    elif target < data[mid]:
      high = mid - 1
    else:
      low = mid + 1
  return False
```

T(n) = 5 * (1 + log n) + 5

T(n) = 5 + 5log n + 5

T(n) = 5log n + 10

T(n) = O(log n)

#### Worst Case


```python
def binary_search(data, target):
  low = 0 # 1
  high = len(data) - 1 # 3

  while low <= high: # 1 (1 + log n)
    mid = (low + high) // 2 # 3(1 + log n)
    if target == data[mid]: # 1(1 + log n)
      return True 
    elif target < data[mid]: # 1 (1 + log n)
      high = mid - 1
    else:
      low = mid + 1 
  return False # 1
```

T(n) = 6 * (1 + log n) + 5

T(n) = 6 + 6log n + 5

T(n) = 6log n + 11

T(n) = O(log n)
