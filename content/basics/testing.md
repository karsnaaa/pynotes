---
title: Testing
date: 2025-06-29
author: Your Name
cell_count: 5
score: 5
---

```python
# created :20250629
```


```python
https://openai.com/chatgpt/overview/
```


```python
def classify_temperature(celsius):
    """
    Classify the temperature in Celsius.

    Parameters:
    celsius (float): Temperature in degrees Celsius.

    Returns:
    str: Classification of the temperature.
    """
    if celsius < 10:
        return "Cold"
    elif 10 <= celsius <= 25:
        return "Moderate"
    else:
        return "Hot"

def main():
    try:
        temp_input = float(input("Enter the temperature in Celsius: "))
        classification = classify_temperature(temp_input)
        print(f"The temperature is classified as: {classification}")
    except ValueError:
        print("Invalid input. Please enter a numeric value.")

if __name__ == "__main__":
    main()
```

    Enter the temperature in Celsius:  42
    

    The temperature is classified as: Hot
    


```python

```


```python

```


---
**Score: 5**