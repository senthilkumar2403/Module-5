# Exp.No:25  
## Hierarchical Inheritance
---
### AIM  
To write a Python program to get the name, attendance and Id of a student and check if they are eligible for the Next Module using multiple inheritance.

---
### ALGORITHM
1. Begin the program.  
2. Create a base class `Student` with an `__init__` method to initialize `name` and `id`.  
3. Create a base class `Attendance` with an `__init__` method to initialize `attendance`.  
4. Create a derived class `Module` that inherits from both `Student` and `Attendance`.  
   - Define an `__init__` method to initialize `name`, `id`, and `attendance`.  
   - Define a method `check_eligibility()` to check if attendance is greater than 80.  
   - If attendance > 80, print `"Eligible for Module Exam"`.  
   - Otherwise, print `"Not Eligible for Module Exam"`.  
5. Accept input for `name`, `id`, and `attendance` from the user.  
6. Create an object of the `Module` class and call `check_eligibility()`.  
7. Terminate the program.

---
### PROGRAM
```python
# Reg.No- 212222060234
# Name- Senthilkumar K
class Student:
    def __init__(self, name, id):
        self.name = name
        self.id = id

class Attendance:
    def __init__(self, attendance):
        self.attendance = attendance

class Module(Student, Attendance):
    def __init__(self, name, id, attendance):
        Student.__init__(self, name, id)
        Attendance.__init__(self, attendance)

    def check_eligibility(self):
        print(self.name)
        print(self.id)
        if self.attendance > 80:
            print("Eligible for Module Exam")
        else:
            print("Not Eligible for Module Exam")

name = input()
id = int(input())
attendance = int(input())
obj = Module(name, id, attendance)
obj.check_eligibility()
```

### OUTPUT
<img width="684" height="284" alt="image" src="https://github.com/user-attachments/assets/23691f16-e6da-4732-96e6-7793861fc2b7" />


### RESULT
Thus, the Python program to check student eligibility for the Next Module using multiple inheritance has been successfully executed and the output is verified.
