---
title: Vowels
date: 2025-07-21
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
vowels = 'aeiou'
ip_str = 'Hello, have you tried our tutorial section yet?'
ip_str = ip_str.casefold()
count = {}.fromkeys(vowels,0)
for char in ip_str:
   if char in count:
       count[char] += 1
print(count)
```


---
**Score: 0**