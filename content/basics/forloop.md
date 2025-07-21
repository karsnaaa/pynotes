---
title: Forloop
date: 2025-07-21
author: Your Name
cell_count: 23
score: 20
---

```python
# Step 1: Import time for delay demo
import time

```


```python

print("📘 Welcome to the Square Generator")

```


```python
# Step 4: Start loop
for i in range(1, 11):

```


```python
    # Loop Step 1
    print(f"🔁 Looping... i = {i}")

```


```python
    # Pause for visibility
    time.sleep(0.2)

```


```python
    # Calculate square
    square = i ** 2

```


```python
    # Print square
    print(f"🔢 Square of {i} is {square}")

```


```python
# After loop: show summary
print("✅ Loop complete")

```


```python
# Now let’s visualize the data
import matplotlib.pyplot as plt

```


```python
x = list(range(1, 11))
y = squares

```


```python
plt.plot(x, y, marker='o')

```


```python
plt.title("Squares of Numbers")

```


```python
plt.xlabel("Number")

```


```python
plt.grid(True)

```


```python
plt.show()

```


```python
# Let's show individual items again for recap

```


```python
for index, value in enumerate(squares):

```


```python
    print(f"{index+1}^2 = {value}")

```


```python
squares2 = [i**2 for i in range(1, 11)]

```


```python
print("Using list comprehension:", squares2)

```


```python
print("🎉 Program Finished!")

```

    🎉 Program Finished!
    


```python

```


```python

```


---
**Score: 20**