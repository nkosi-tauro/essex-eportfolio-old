---
layout: page
title: Unit 5 - More on Classes
permalink: /unit5/
---

## Python Program
- **Instructions**: Write a Python program with polymorphism that is usable within the summative assessment for the driverless car.

```py
# Driverless Car - Polymorphism
class Car:
  def __init__(self, make, model, range_km, year):
    self.make = make
    self.model = model
    self.range_km = range_km
    self.year = year

  def switch_car_on(self):
    print(f"The {self.make} AI is now switching the car on")
        
  def stop_car(self):
    print(f"The {self.make} AI is now stopping the car")
        
  def accelerate_car(self):
    print(f"The {self.make} AI is now accelerating the car you have {self.range_km}km left")
        
  def brake_car(self):
    print(f"The {self.make} AI is now braking the car")

class ElectricCar(Car):
  def __init__(self, make, model, range_km, year):
    super().__init__(make, model, range_km, year)

  def switch_car_on(self):
    print(f"The {self.make} AI is now switching the car on")
  
  def stop_car(self):
    print(f"The {self.make} AI is now stopping the car")
  
  def accelerate_car(self):
    print(f"The {self.make} AI is now accelerating the car you have {self.range_km}km left")
  
  def brake_car(self):
    print(f"The {self.make} AI is now braking the car")

# create an instance of the ElectricCar class
car1 = Car("Tesla", "Model S", 500, 2020)
# print the car details
print(f"I am a {car1.make} {car1.model}, my range is {car1.range_km}km and I was made in {car1.year}")
# switch the car on
car1.switch_car_on()
# accelerate the car
car1.accelerate_car()
# brake the car
car1.brake_car()
# stop the car
car1.stop_car()
```