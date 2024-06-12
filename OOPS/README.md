Let's start with the basics of Object-Oriented Programming (OOP) in Python, focusing on the parent (base) and child (derived) class relationships. We'll cover the following concepts:

1. [What is a class?](#what-is-a-class)



### 1. What is a Class?

A class is a blueprint for creating objects. Objects have properties (attributes) and behaviors (methods).

### Example:
```python
class Animal:
    def __init__(self, name, species):
        self.name = name
        self.species = species

    def make_sound(self):
        print(f"{self.name} makes a sound.")
```

In this example, `Animal` is a class with an `__init__` method to initialize the name and species, and a method `make_sound` that prints a message.

### 2. What is Inheritance?

Inheritance allows a class (child class) to inherit attributes and methods from another class (parent class). This helps in reusing code and creating a hierarchical relationship between classes.


