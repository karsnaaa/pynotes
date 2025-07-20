---
title: Hcf
date: 2025-07-21
author: Your Name
cell_count: 7
score: 5
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
    



```


```python
for i in range(1, smaller+1):
        if((x % i == 0) and (y % i == 0)):
            hcf = i 
    return hcf
```


```python
num1 = 54 
```


```python
num2 = 24
```


```python
print("The H.C.F. is", compute_hcf(num1, num2))
```


---
**Score: 5**