---
title: Prime Numbers
date: 2025-07-20
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
num = 29
flag = False
if num == 0 or num == 1:
    print(num, "is not a prime number")
elif num > 1:
    for i in range(2, num):
        if (num % i) == 0:
            flag = True
            break
    if flag:
        print(num, "is not a prime number")
    else:
        print(num, "is a prime number")
```


---
**Score: 0**