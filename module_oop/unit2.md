---
layout: page
title: "Unit 2: Object Oriented Analysis - Initial Steps towards Programming in Python"
permalink: module_oop/unit2/
---

## Python Program
- Write a Python program to achieve basic employee-related functionality which includes retaining employee details and allowing an employee to book a day of annual leave. Extend the Python program you have now created to use protected and unprotected variables.

```py
# Employee details and annual leave
class Employee():

  def __init__(self, name, surname, empID, leave):
    self.name = name # unprotected variable
    self.surname = surname # unprotected variable
    self._empID = empID # protected variable
    self._leave = leave # protected variable

  def scheduleLeave(self, days):
    if days <= self._leave:
      self._leave -= days
      print("You have scheduled annual leave")
    else:
      print("You have taken too much leave")
  

# Create an instance of the Employee class
employee1 = Employee("Nkosi", "T", "1234", 20)
# Print the employee details
print(f"I am {employee1.name} {employee1.surname}, my employee ID is {employee1._empID} and I have {employee1._leave} days of annual leave left")
# Book annual leave
employee1.scheduleLeave(21)
```

---