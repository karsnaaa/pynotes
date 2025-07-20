---
title: Dsa
date: 2025-07-21
author: Your Name
cell_count: 148
score: 145
---

```python
print("📘 Data Structures and Algorithms (DSA) in Python - 200 Cells")
```


```python
arr = [3, 1, 4, 1, 5, 9, 2, 6, 5]
```


```python
print('Original array:', arr)
```


```python
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n-i-1):
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]
```


```python
arr_copy = arr[:]
bubble_sort(arr_copy)
print('Bubble sorted:', arr_copy)
```


```python
def selection_sort(arr):
    n = len(arr)
    for i in range(n):
        min_idx = i
        for j in range(i+1, n):
            if arr[j] < arr[min_idx]:
                min_idx = j
        arr[i], arr[min_idx] = arr[min_idx], arr[i]
```


```python
arr_copy2 = arr[:]
selection_sort(arr_copy2)
print('Selection sorted:', arr_copy2)
# %%
# Cell 8
def linear_search(arr, x):
    for i in range(len(arr)):
        if arr[i] == x:
            return i
    return -1
```


```python
print('Index of 5:', linear_search(arr, 5))
```


```python
def binary_search(arr, x):
    l, r = 0, len(arr)-1
    while l <= r:
        mid = (l + r) // 2
        if arr[mid] == x:
            return mid
        elif arr[mid] < x:
            l = mid + 1
        else:
            r = mid - 1
    return -1
```


```python
sorted_arr = sorted(arr)
print('Binary Search for 5:', binary_search(sorted_arr, 5))
```


```python
stack = []
stack.append(10)
stack.append(20)
print('Stack pop:', stack.pop())
```


```python
from collections import deque
queue = deque()
queue.append(10)
queue.append(20)
print('Queue pop:', queue.popleft())
```


```python
def factorial(n):
    return 1 if n == 0 else n * factorial(n-1)
```


```python
print('Factorial of 5:', factorial(5))
```


```python
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n-1) + fibonacci(n-2)
```


```python
print('Fibonacci of 6:', fibonacci(6))
```


```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
```


```python
class LinkedList:
    def __init__(self):
        self.head = None

    def append(self, data):
        new_node = Node(data)
        if not self.head:
            self.head = new_node
            return
        last = self.head
        while last.next:
            last = last.next
        last.next = new_node

    def print_list(self):
        curr = self.head
        while curr:
            print(curr.data, end=' -> ')
            curr = curr.next
        print('None')
```


```python
ll = LinkedList()
ll.append(1)
ll.append(2)
ll.append(3)
ll.print_list()
```


```python
def square_20(x):
    return x * x
print('Square of 20:', square_20(20))
```


```python
def square_21(x):
    return x * x
print('Square of 21:', square_21(21))
```


```python
def square_22(x):
    return x * x
print('Square of 22:', square_22(22))
```


```python
def square_23(x):
    return x * x
print('Square of 23:', square_23(23))
```


```python
def square_24(x):
    return x * x
print('Square of 24:', square_24(24))
```


```python
def square_25(x):
    return x * x
print('Square of 25:', square_25(25))
```


```python
def square_26(x):
    return x * x
print('Square of 26:', square_26(26))
```


```python
def square_27(x):
    return x * x
print('Square of 27:', square_27(27))
```


```python
def square_28(x):
    return x * x
print('Square of 28:', square_28(28))
```


```python
def square_29(x):
    return x * x
print('Square of 29:', square_29(29))
```


```python
def square_30(x):
    return x * x
print('Square of 30:', square_30(30))
```


```python
def square_31(x):
    return x * x
print('Square of 31:', square_31(31))
```


```python
def square_32(x):
    return x * x
print('Square of 32:', square_32(32))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(34))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(35))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(36))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(37))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(38))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(39))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(40))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(41))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(42))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(43))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(44))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(45))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(46))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(50))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(51))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(52))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(53))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(54))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(55))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))def square_33(x)
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))def square_33(x)
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))def square_33(x)
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


```python
def square_33(x):
    return x * x
print('Square of 33:', square_33(33))
```


---
**Score: 145**