# OOPS_Python
# Encapsulation Example in Python

## 📌 Description

This repository contains a simple example of **Encapsulation** in Python.  
Encapsulation is one of the fundamental principles of Object-Oriented Programming (OOP), which refers to **binding data members (variables) and member functions (methods) inside a single unit (class)**.  
It also helps in **data hiding**, restricting direct access to some of an object's components, which is useful for preventing accidental modification of data.

---

## 📚 What is Encapsulation?

- **Encapsulation** means wrapping the data (variables) and code (methods) together as a single unit.
- In Python, we achieve encapsulation by using **private variables** (prefixing variable names with `__`).
- It helps in **data hiding** and provides control over the data by **getters** and **setters**.

---

## 💻 Code Example

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

---



## 📧 Contact
Saubhaggya Srivastava
For any queries, contact me at [saubhaggya321@gmail.com]  


> **Note:** Replace `your-username`, `your-repo-name`, and `your-email@example.com` with your actual details before uploading.
