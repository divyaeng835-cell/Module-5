# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM

1. **Begin the program.**
2. **Create a class Details** with an `__init__` method to initialize three attributes: `id`, `name`, and `gender`.
3. **Define a method display_details()** to print the values of `id`, `name`, and `gender`.
4. **Create a class Employee** that inherits from the `Details` class. 
   - Add two additional attributes: `company` and `department`.
   - Override the `display_details()` method to print the employee-specific attributes (`company` and `department`) along with the inherited details.
5. **Create a class Doctor** that also inherits from the `Details` class. 
   - Add two additional attributes: `hospital` and `department`.
   - Override the `display_details()` method to print the doctor-specific attributes (`hospital` and `department`) along with the inherited details.
6. **Accept input** for employee and doctor details.
7. **Create objects of Employee and Doctor** using the input.
8. **Call the `display_details()` method** for both objects to print the details.
9. **Terminate the program.**

---

### PROGRAM
```
class Details:
    def _init_(self, id, name, gender):
        self.id = id
        self.name = name
        self.gender = gender

    def show_details(self):
        print(f"Id: {self.id}")
        print(f"Name: {self.name}")
        print(f"Gender: {self.gender}")

class Employee(Details):
    def _init_(self, id, name, gender, company, department):
        super()._init_(id, name, gender)
        self.company = company
        self.department = department

    def show_details(self):
        print("Employee Object")
        super().show_details()
        print(f"Company: {self.company}")
        print(f"Department: {self.department}")

class Doctor(Details):
    def _init_(self, id, name, gender, hospital, department):
        super()._init_(id, name, gender)
        self.hospital = hospital
        self.department = department

    def show_details(self):
        print("Doctor Object")
        super().show_details()
        print(f"Hospital: {self.hospital}")
        print(f"Department: {self.department}")

# Getting input for Employee
id1 = int(input())
name1 = input()
gender1 = input()
company = input()
department1 = input()
emp = Employee(id1, name1, gender1, company, department1)
emp.show_details()

# Getting input for Doctor
id2 = int(input())
name2 = input()
gender2 = input()
hospital = input()
department2 = input()
doc = Doctor(id2, name2, gender2, hospital, department2)
doc.show_details()
```

### OUTPUT  
![Screenshot 2025-04-28 093654](https://github.com/user-attachments/assets/3fdbc484-3ad8-4b67-89b3-82fde4da0765)
### RESULT
Thus the python program to get the employee and doctor details and display using hierarchical inheritance has been implemented successfully.
