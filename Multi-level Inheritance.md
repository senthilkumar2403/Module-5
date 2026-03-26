# Exp.No:24  
## Multi-level Inheritance
---
### AIM  
To write a Python program to get the name, age and ID of a person and display them using Multilevel Inheritance.

---
### ALGORITHM
1. Define the `Person` class with an `__init__` method that initializes `name` and `age`.  
2. Define the `PersonDetails` class that inherits from `Person` with an `__init__` method that initializes `name`, `age`, and `person_id` using `super()`.  
3. Define the `DisplayDetails` class that inherits from `PersonDetails` with an `__init__` method that calls `super()` to initialize all attributes.  
4. Define a `show_details()` method inside `DisplayDetails` that prints `name`, `age`, and `person_id`.  
5. Accept `name`, `age`, and `person_id` from the user.  
6. Create an instance of `DisplayDetails` and call `show_details()`.  
7. Terminate the program.

---
### PROGRAM
```python
# Reg.No- 212222060234
# Name- Senthilkumar K
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

class PersonDetails(Person):
    def __init__(self, name, age, person_id):
        super().__init__(name, age)
        self.person_id = person_id

class DisplayDetails(PersonDetails):
    def __init__(self, name, age, person_id):
        super().__init__(name, age, person_id)

    def show_details(self):
        print(self.name, self.age, self.person_id)

name = input()
age = int(input())
person_id = int(input())
person = DisplayDetails(name, age, person_id)
person.show_details()
```

### OUTPUT
<img width="545" height="204" alt="image" src="https://github.com/user-attachments/assets/80b499bf-aec1-493f-b5ca-63537e186937" />


### RESULT
Thus, the Python program to get the name, age and ID of a person and display them using Multilevel Inheritance has been successfully executed and the output is verified.
