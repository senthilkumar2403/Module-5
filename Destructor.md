# Exp.No:22  
## Destructor
---
### AIM  
To create a Python program with a destructor and print a message when an object of the class is created, and after the program execution print a message that the object is deleted.

---
### ALGORITHM
1. Begin the program.  
2. Define the `Employee` class.  
3. Inside the `Employee` class, define the `__init__` method (constructor) that prints `"Employee created."`.  
4. Define the `__del__` method (destructor) that prints `"Destructor called, Employee deleted."`.  
5. Create an object `obj` of the `Employee` class. This triggers the constructor.  
6. When the program ends, the destructor is automatically called and the object is deleted.  
7. Terminate the program.

---
### PROGRAM
```python
# Reg.No- 212222060234
# Name- Senthilkumar K
class Employee:
    def __init__(self):
        print("Employee created.")

    def __del__(self):
        print("Destructor called, Employee deleted.")

obj = Employee()
del obj
```

### OUTPUT
<img width="684" height="168" alt="image" src="https://github.com/user-attachments/assets/d7a14928-4c1c-49e7-96cd-ffe2acc9172e" />


### RESULT
Thus, the Python program to demonstrate the use of a destructor in a class has been successfully executed and the output is verified.
