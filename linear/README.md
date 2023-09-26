# Linear

This is when the resource needed and the data being processed grows at the same rate.

## Examples

```python
def linear(data):
  for i in range(len(data)): # 1 + 1 + n
    return data[i] # 1(n) = n
```

T(n) = 1 + 1 + n + n

T(n) = 2n + 2

T(n) = O(n)

```python
def linear_search(my_list, key):
    for i in range(0, len(my_list)): # n - 1 + 1 + 1 = n + 1
        if my_list[i] == key: # 1(n + 1)
            return i # 1
```

T(n) = n + 1 + 1(n + 1) + 1

T(n) = n + 1 + n + 1 + 1

T(n) = 2n + 3

T(n) = O(n)

```python
def function1(number):
 total=0; # 1

 for i in range(0,number): # n + 1
  x = (i + 1) # 2n
  total += (x * x) # 2n

 return total # 1
```

T(n) = 1 + (n + 1) + 2n + 2n + 1

T(n) = 5n + 3

T(n) = O(n)
