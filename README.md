# OOPS_Python

## 📌 Description

This repository contains simple and clear examples of **Encapsulation** and **Abstraction** in Python.  
Both are fundamental principles of **Object-Oriented Programming (OOP)** that help in organizing code, hiding complexity, and securing data.

---

## 📚 What is Encapsulation?

- **Encapsulation** means wrapping the data (variables) and code (methods) together as a single unit called a **class**.
- It restricts direct access to some of an object's components, using **private variables**.
- Encapsulation helps in **data hiding** and provides controlled access to the data using **getter** and **setter** methods.

---

## 💻 Encapsulation Example

```python
# Encapsulation Example

class Date:
    def __init__(self, dd, mm, yy):
        # Private data members
        self.__dd = dd
        self.__mm = mm
        self.__yy = yy

    # Public method to access private data
    def get(self):
        print(f"Date is: {self.__dd}/{self.__mm}/{self.__yy}")

# Object creation
d1 = Date(10, 11, 2003)
d1.get()  # Output: Date is: 10/11/2003
```

### ✅ Output

```
Date is: 10/11/2003
```

---

## 📚 What is Abstraction?

- **Abstraction** is used to **hide complex implementation** and **show only essential features** to the user.
- In Python, **Abstract Base Classes (ABC)** and **abstract methods** are used to implement abstraction.
- It focuses on **what to do**, not **how to do**.

---

## 💻 Abstraction Example

```python
# Abstraction Example

from abc import ABC, abstractmethod

# Abstract Class
class Shape(ABC):

    @abstractmethod
    def draw(self):
        pass

    @abstractmethod
    def area(self):
        pass

# Class Rectangle(Concrete Classes)
class Rectangle(Shape):

    def draw(self):
        print("Drawing a Rectangle")

    def area(self, length, breadth):
        return length * breadth

# Class Circle(Concrete Classes)
class Circle(Shape):

    def draw(self):
        print("Drawing a Circle")

    def area(self, radius):
        return 3.14 * radius * radius

# Object creation and method calls
r1 = Rectangle()
r1.draw()
areaR = r1.area(2, 3)
print(areaR)

c1 = Circle()
c1.draw()
areaC = c1.area(5)
print(areaC)
```

### ✅ Output

```
Drawing a Rectangle
6
Drawing a Circle
78.5
```

---

## 📧 Contact

**Saubhaggya Srivastava**  
For any queries, contact me at [saubhaggya321@gmail.com]  


