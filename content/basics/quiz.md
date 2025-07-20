---
title: Quiz
date: 2025-07-21
author: Your Name
cell_count: 4
score: 0
---

```python
# created :20250629
```


```python
https://openai.com/chatgpt/overview/
```


```python
import random

def ask_question():
    """Ask a random addition question, return True if correct."""
    a = random.randint(1, 10)
    b = random.randint(1, 10)
    try:
        answer = int(input(f"What is {a} + {b}? "))
    except ValueError:
        print("Please enter a valid number.")
        return False

    if answer == a + b:
        print("✅ Correct!")
        return True
    else:
        print(f"❌ Incorrect. The right answer is {a + b}.")
        return False

def quiz(num_questions=10):
    """Run the quiz for a fixed number of questions."""
    score = 0  # important: initialize once outside loop
    for i in range(1, num_questions + 1):
        print(f"\nQuestion {i}/{num_questions}")
        if ask_question():
            score += 1
    print(f"\n🎉 Quiz complete! Your score: {score}/{num_questions}")

if __name__ == "__main__":
    quiz()
```

    
    Question 1/10
    

    What is 6 + 1?  7
    

    ✅ Correct!
    
    Question 2/10
    

    What is 10 + 10?  20
    

    ✅ Correct!
    
    Question 3/10
    

    What is 7 + 7?  14
    

    ✅ Correct!
    
    Question 4/10
    

    What is 5 + 1?  6
    

    ✅ Correct!
    
    Question 5/10
    

    What is 2 + 7?  
    

    Please enter a valid number.
    
    Question 6/10
    

    What is 7 + 8?  9
    

    ❌ Incorrect. The right answer is 15.
    
    Question 7/10
    

    What is 7 + 5?  12
    

    ✅ Correct!
    
    Question 8/10
    

    What is 3 + 5?  8
    

    ✅ Correct!
    
    Question 9/10
    

    What is 3 + 5?  8
    

    ✅ Correct!
    
    Question 10/10
    

    What is 7 + 9?  16
    

    ✅ Correct!
    
    🎉 Quiz complete! Your score: 8/10
    


```python

```


---
**Score: 0**