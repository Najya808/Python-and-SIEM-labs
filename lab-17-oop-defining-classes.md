What I Learned

In this lab, I learned the fundamentals of Object-Oriented Programming (OOP) in Python. I practiced creating classes, defining instance and class attributes, and instantiating objects. I also explored how methods encapsulate behavior and how instance attributes differ from class attributes, which are shared across all objects of a class.

🎯 Lab Objectives

Understand the basics of OOP by defining and using classes

Differentiate between instance attributes and class attributes

Create and manipulate objects in Python

Apply methods to objects to define behavior

📋 Prerequisites

Basic understanding of programming concepts

Familiarity with Python syntax

🧪 Lab Tasks Performed

🔹 Task 1: Define a Class Car

Objective: Create a class and define attributes and methods.

class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

    def drive(self):
        print(f"The {self.brand} {self.model} is now driving.")


 Explanation

__init__ initializes instance attributes for each object

drive() is a method representing behavior of the object

self refers to the individual object instance

🔹 Task 2: Instantiate Car Objects

Objective: Create and use objects from the Car class

car1 = Car("Toyota", "Corolla")
car2 = Car("Honda", "Civic")

car1.drive()
car2.drive()

print(f"Car 1 brand: {car1.brand}")
print(f"Car 2 brand: {car2.brand}")


🔍 Explanation

car1 and car2 are instances of Car

Each object maintains its own attributes (brand, model)

Methods can be called on each object to perform actions

🔹 Task 3: Instance Attributes vs Class Attributes

Objective: Understand the difference between shared and unique attributes

class Car:
    wheels = 4  # Class attribute
    
    def __init__(self, brand, model):
        self.brand = brand  # Instance attribute
        self.model = model

    def drive(self):
        print(f"The {self.brand} {self.model} is now driving.")

# Accessing class attribute
print(f"Number of wheels: {Car.wheels}")


🔍 Explanation

Instance Attributes: Unique to each object (brand, model)

Class Attributes: Shared across all objects of the class (wheels)

Class attributes are accessed using ClassName.attribute

🧩 Key Concepts Covered

Definition and initialization of a class

Creation and manipulation of objects

Instance vs class attributes

Encapsulation of behavior using methods

 Conclusion

In this lab, I successfully:

Created a Python class and instantiated objects

Used methods to define object behavior

Differentiated between instance attributes and class attributes

These OOP fundamentals are essential for designing organized, reusable, and maintainable code, and they lay the foundation for advanced concepts like inheritance, polymorphism, and abstraction.
