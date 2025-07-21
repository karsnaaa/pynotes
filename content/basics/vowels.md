---
title: Vowels
date: 2025-07-21
author: Your Name
cell_count: 8
score: 5
---

```python
# created :20250629
```


```python
https://share.google/camtfs4z8aiYAJNSz
```


```python
vowels = 'aeiou'
```


```python
ip_str = 'Hello, have you tried our tutorial section yet?'
```


```python
ip_str = ip_str.casefold()
```


```python
count = {}.fromkeys(vowels,0)
```


```python
for char in ip_str:
   if char in count:
       count[char] += 1
```


```python
print(count)
```


---
**Score: 5**