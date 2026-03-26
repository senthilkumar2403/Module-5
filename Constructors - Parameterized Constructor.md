# Exp.No:21  
## Constructors - Parameterized Constructor
---
### AIM  
To write a Python program using a class to perform addition of two numbers using a parameterized constructor.

---
### ALGORITHM
1. Begin the program.  
2. Define a class `Addition`.  
3. The class should have a parameterized `__init__` method that accepts two parameters: `a` and `b`.  
4. Inside the `__init__` method, assign the values to `self.a` and `self.b`.  
5. Define a method `add(self)` to perform and print the addition of `self.a` and `self.b`.  
6. Prompt the user to enter two numbers.  
7. Create an instance of the class by passing the entered numbers to the constructor.  
8. Call the `add()` method to display the result.  
9. Terminate the program.

---
### PROGRAM
```python
# Reg.No- 212222060234
# Name- Senthilkumar K
class Addition:
    def __init__(self, a, b):
        self.a = a
        self.b = b
        print("First number =", self.a)
        print("Second number =", self.b)

    def add(self):
        print("Addition of two numbers =", self.a + self.b)

a = int(input())
b = int(input())
obj = Addition(a, b)
obj.add()
```

### OUTPUT
<img width="684" height="279" alt="image" src="https://github.com/user-attachments/assets/2e9bddf0-d13d-47a0-b362-28d9c1d10a32" />

### RESULT
Thus, the Python program to perform addition of two numbers using a parameterized constructor has been successfully executed and the output is verified.
