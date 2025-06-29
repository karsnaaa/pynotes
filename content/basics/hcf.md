---
title: Hcf
date: 2025-06-29
author: Your Name
cell_count: 3
score: 0
---

```python
# created :20250629
```


```python
https://share.google/camtfs4z8aiYAJNSz
```


```python
def compute_hcf(x, y):
    if x > y:
        smaller = y
    else:
        smaller = x
    for i in range(1, smaller+1):
        if((x % i == 0) and (y % i == 0)):
            hcf = i 
    return hcf
num1 = 54 
num2 = 24
print("The H.C.F. is", compute_hcf(num1, num2))
```


---
**Score: 0**