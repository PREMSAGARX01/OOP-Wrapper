PR 5 - OOP Wrapper

Employee Management System

Objective

The purpose of this project is to develop an Employee Management System using Object-Oriented Programming (OOP) concepts in Python. The system demonstrates the use of classes, inheritance, encapsulation, method overloading, method overriding, constructors, destructors, and menu-driven programming.


Features

- Add Employees
- Add Managers
- Add Developers
- Display Employee Details
- Display Manager Details
- Display Developer Details
- Update Employee Salary
- Update Employee ID
- Remove Employees
- Check Class Inheritance using "issubclass()"
- Menu-Driven Interface


OOP Concepts Implemented

1. Class and Object

Classes used:

- Person
- Employee
- Manager
- Developer

Objects are created dynamically through user input.


2. Constructor

The "__init__()" constructor is used to initialize object attributes.

Example:

def __init__(self, name, age):
    self.name = name
    self.age = age


3. Destructor

The "__del__()" method is used as a destructor.

Example:

def __del__(self):
    pass


4. Encapsulation

Sensitive attributes are declared private using double underscores.

self.__employee_id
self.__salary

Access is provided through getter and setter methods.


5. Getter and Setter Methods

Getter Methods:

get_employee_id()
get_salary()

Setter Methods:

set_employee_id()
set_salary()


6. Inheritance

The Manager and Developer classes inherit from Employee.

class Manager(Employee):

class Developer(Employee):


7. Method Overriding

The "display()" method is overridden in both Manager and Developer classes.


8. Method Overloading (Python Style)

Python does not support true method overloading. It is simulated using default parameters.

def __init__(
    self,
    employee_id="NA",
    name="Unknown",
    age=0,
    salary=0
):


9. super()

The "super()" function is used to call parent class constructors.

super().__init__(
    employee_id,
    name,
    age,
    salary
)


10. issubclass()

Used to verify inheritance relationships.

issubclass(Manager, Employee)
issubclass(Developer, Employee)


Project Structure

Person
   |
Employee
   |
   +-- Manager
   |
   +-- Developer


Menu Options

1. Add Employee
2. Add Manager
3. Add Developer
4. Display Employees
5. Display Managers
6. Display Developers
7. Update Salary
8. Update Employee ID
9. Remove Employee
10. Check Inheritance
11. Exit


Sample Output

===== EMPLOYEE MANAGEMENT SYSTEM =====

1. Add Employee
2. Add Manager
3. Add Developer
4. Display Employees
5. Display Managers
6. Display Developers
7. Update Salary
8. Update Employee ID
9. Remove Employee
10. Check Inheritance
11. Exit


Requirements

- Python 3.x


How to Run

1. Download the project files.
2. Open Terminal or Command Prompt.
3. Navigate to the project folder.
4. Run:

python oop_wrapper.py

Assumptions

- Employee IDs are assumed to be unique.
- Salary values are entered as numeric values.
- Managers belong to a department.
- Developers have a programming language specialization.


Author

Name: Premsagar Meena 
Project: OOP Wrapper
