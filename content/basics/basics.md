---
title: Basics
date: 2025-07-21
author: Your Name
cell_count: 54
score: 50
---

```python
# Cell 1
a = 10

```


```python
# Cell 2
b = 20

```


```python
# Cell 3
c = a + b
print(c)

```


```python
# Cell 4
for i in range(5):
    print(i)

```


```python
# Cell 5
def square(x):
    return x * x

```


```python
class Person:
    pass
```


```python
p1 = Person()
print(type(p1))
```


```python
<class '__main__.Person'>
```


```python
class Student:
    def __init__(self, name, age):
        self.name = name
        self.age = age
```


```python
s1 = Student("Sara", 20)
print(s1.name, s1.age)
```


```python
class Dog:
    def __init__(self, breed):
        self.breed = breed

    def bark(self):
        print("Woof! I am a", self.breed)
```


```python
d = Dog("Labrador")
d.bark()
```


```python
class Book:
    def __init__(self, title):
        self.title = title

    def __str__(self):
        return f"Book: {self.title}"
```


```python
b = Book("Harry Potter")
print(b)
```


```python
class Animal:
    def __init__(self, name):
        self.name = name

    def speak(self):
        print("I am an animal.")
```


```python
class Cat(Animal):
    def speak(self):
        print(f"{self.name} says Meow!")
```


```python
c = Cat("Luna")
c.speak()
```


```python
class Parent:
    def __init__(self):
        print("Parent init")
```


```python
class Child(Parent):
    def __init__(self):
        super().__init__()
        print("Child init")
```


```python
c = Child()
```


```python
Parent init
Child init
```


```python
class Account:
    def __init__(self, balance):
        self.__balance = balance  # private

    def show_balance(self):
        print("Balance:", self.__balance)
```


```python
acc = Account(1000)
acc.show_balance()
```


```python
class BankAccount:
    def __init__(self, name, balance):
        self.name = name
        self.__balance = balance

    def deposit(self, amount):
        self.__balance += amount

    def withdraw(self, amount):
        if amount <= self.__balance:
            self.__balance -= amount
        else:
            print("Insufficient funds")

    def show(self):
        print(f"{self.name} has ₹{self.__balance}")
```


```python
user1 = BankAccount("Sara", 5000)
user1.show()
```


```python
user1.deposit(2000)
user1.show()
```


```python
user1.withdraw(3000)
user1.show()
```


```python
class MathOps:
    @staticmethod
    def add(a, b):
        return a + b
```


```python
print(MathOps.add(5, 7))
```


```python
class Student:
    school = "CodeHigh"

    @classmethod
    def get_school(cls):
        return cls.school
```


```python
print(Student.get_school())
```


```python
class Calculator:
    def add(self, a: int, b: int) -> int:
        """Returns the sum of two numbers."""
        return a + b
calc = Calculator()
```


```python
print(calc.add(2, 3))
```


```python
class Vehicle:
    def __init__(self, name):
        self.name = name

    def drive(self):
        print(f"{self.name} is driving.")
```


```python
class Car(Vehicle):
    def drive(self):
        print(f"{self.name} (car) is zooming!")
```


```python
class Bike(Vehicle):
    def drive(self):
        print(f"{self.name} (bike) is vrooming!")
```


```python
v = Vehicle("Generic")
v.drive()

c = Car("Suzuki")
c.drive()

b = Bike("Yamaha")
b.drive()
```


```python
class Student:
    def __init__(self, name):
        self.__name = name

    def get_name(self):
        return self.__name

    def set_name(self, new_name):
        self.__name = new_name
```


```python
s = Student("Sara")
print(s.get_name())
s.set_name("Queen Sara")
print(s.get_name())
```


```python
class Book:
    def __init__(self, title):
        self.title = title
        self.available = True
```


```python
class Library:
    def __init__(self):
        self.books = []

    def add_book(self, book):
        self.books.append(book)

    def show_books(self):
        for book in self.books:
            status = "Available" if book.available else "Issued"
            print(f"{book.title} - {status}")

    def issue_book(self, title):
        for book in self.books:
            if book.title == title and book.available:
                book.available = False
                print(f"{title} has been issued.")
                return
        print(f"{title} is not available.")
```


```python
lib = Library()
book1 = Book("Harry Potter")
book2 = Book("Sherlock Holmes")
lib.add_book(book1)
lib.add_book(book2)
```


```python
lib.show_books()
```


```python
lib.issue_book("Harry Potter")
lib.show_books()
```


```python
class Employee:
    def __init__(self, name, salary):
        self.name = name
        self.salary = salary
```


```python
employees = [
    Employee("Sara", 70000),
    Employee("Ali", 65000),
    Employee("Afia", 72000)
]

for emp in employees:
    print(f"{emp.name} earns ₹{emp.salary}")
```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


---
**Score: 50**