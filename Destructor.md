# Exp.No:22  
## Destructor

---

### AIM  
To create a Python class `Student` with a destructor.

---

### ALGORITHM

1. Begin the program.  
2. Define the `student` class.  
3. Inside the `student` class, define the `__init__` method (constructor) and the `__del__` method (destructor).  
4. Create an object `s` of the `student` class. When the object `s` is created, the `__init__` method is called, and its print statements are executed.  
5. Use the `del` statement to delete the object `s`. This triggers the `__del__` method (destructor), and the respective print statements are executed.  
6. Terminate the program.

---

### PROGRAM

```
class Student:
    def _init_(self, name):
        print("Inside Constructor")
        self.name = name
        print("Object initialized")
    
    def show(self):
        print(f"Hello, my name is {self.name}")
    
    def _del_(self):
        print("Inside destructor")
        print("Object destroyed")

# Creating object
s = Student("Emma")
s.show()

# Deleting object
del s

```

### OUTPUT
![Screenshot 2025-04-28 092309](https://github.com/user-attachments/assets/e42da4da-5597-4b01-a57b-cbf7f68e6bc8)
### RESULT
Thus the python program to create a class `Student` with a destructor has been implemented successfully.
