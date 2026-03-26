# Exp.No:23  
## Multiple Inheritance
---
### AIM  
To write a Python program to calculate Addition, Subtraction and Division using Multiple Inheritance.

---
### ALGORITHM
1. Begin the program.  
2. Define a class `Add` with an `__init__` method that accepts `a` and `b` and a method `add()` that returns `a + b`.  
3. Define a class `Sub` with an `__init__` method that accepts `a` and `b` and a method `sub()` that returns `a - b`.  
4. Define a class `Div` with an `__init__` method that accepts `a` and `b` and a method `div()` that returns `a / b`.  
5. Define a class `Calculate` that inherits from `Add`, `Sub`, and `Div`.  
   - Define an `__init__` method to initialize `a` and `b`.  
   - Call the `add()`, `sub()`, and `div()` methods and print the results.  
6. Accept two numbers from the user.  
7. Create an object of the `Calculate` class and display the results.  
8. Terminate the program.

---
### PROGRAM
```python
# Reg.No- 212222060154
# Name- Mugilan J
class Add:
    def __init__(self, a, b):
        self.a = a
        self.b = b
    def add(self):
        return self.a + self.b

class Sub:
    def __init__(self, a, b):
        self.a = a
        self.b = b
    def sub(self):
        return self.a - self.b

class Div:
    def __init__(self, a, b):
        self.a = a
        self.b = b
    def div(self):
        return self.a / self.b

class Calculate(Add, Sub, Div):
    def __init__(self, a, b):
        self.a = a
        self.b = b

a = int(input())
b = int(input())
obj = Calculate(a, b)
print(obj.add())
print(obj.sub())
print(obj.div())
```

### OUTPUT
<img width="406" height="200" alt="image" src="https://github.com/user-attachments/assets/73ed4b94-533d-4fee-81b5-0228bf5a8e3e" />


### RESULT
Thus, the Python program to calculate Addition, Subtraction and Division using Multiple Inheritance has been successfully executed and the output is verified.
