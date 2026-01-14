What I Learned

In this lab, I learned how inheritance works in Python’s Object-Oriented Programming (OOP). I practiced creating a subclass from a base class, adding new attributes and methods, and overriding parent class methods to extend functionality. I also learned how to use the super() function to access and reuse methods from the parent class, which helps in building modular and reusable code.

 Lab Objectives

Understand the concept of inheritance in OOP

Extend an existing class to create a subclass

Override methods in a subclass for specialized behavior

Use the super() function to call parent class methods

📋 Prerequisites

Basic understanding of Python programming

Familiarity with defining classes and methods

🧪 Lab Tasks Performed

🔹 Task 1: Create a Base Class Car

Objective: Define a base class with basic attributes and methods.

class Car:
    def __init__(self, make, model, year):
        self.make = make
        self.model = model
        self.year = year
    
    def describe_car(self):
        print(f"{self.year} {self.make} {self.model}")


🔍 Explanation

Car class has attributes: make, model, year

describe_car() prints car details

Acts as a blueprint for any car object

🔹 Task 2: Extend the Car Class with Inheritance

Objective: Create a subclass ElectricCar that inherits from Car and adds a new attribute.

class ElectricCar(Car):
    def __init__(self, make, model, year, battery_size=75):
        super().__init__(make, model, year)
        self.battery_size = battery_size

    def describe_battery(self):
        print(f"This car has a {self.battery_size}-kWh battery.")


🔍 Explanation

ElectricCar inherits attributes and methods from Car

Uses super() to call the parent class initializer

Adds a new attribute battery_size with default value 75

Introduces a new method describe_battery()

🔹 Task 3: Override a Method in Subclass

Objective: Extend functionality of the parent class method.

class ElectricCar(Car):
    def __init__(self, make, model, year, battery_size=75):
        super().__init__(make, model, year)
        self.battery_size = battery_size

    def describe_car(self):
        super().describe_car()
        self.describe_battery()


🔍 Explanation

describe_car() in ElectricCar overrides the parent method

Calls parent describe_car() using super()

Adds battery information via describe_battery()

Demonstrates method overriding and reuse

🔹 Task 4: Use the Subclass

Objective: Instantiate ElectricCar and call inherited and overridden methods.

my_tesla = ElectricCar('Tesla', 'Model S', 2022)
my_tesla.describe_car()


Expected Output:

2022 Tesla Model S
This car has a 75-kWh battery.


🔍 Explanation

Demonstrates inheritance, method overriding, and adding new functionality

my_tesla object can access both parent and child methods

🧩 Key Concepts Covered

Inheritance allows subclasses to reuse code from a parent class

Method overriding enables custom behavior in subclasses

super() function calls parent class methods for code reuse

Subclasses can introduce new attributes and methods

 Conclusion

In this lab, I successfully:

Created a base class Car and a subclass ElectricCar

Applied inheritance to reuse and extend functionality

Overrode methods to provide specialized behavior

Used super() to access and extend parent methods

Mastering inheritance is essential for modular, maintainable, and reusable OOP code. These skills are crucial for designing scalable Python applications.
