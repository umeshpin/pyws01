Python is an object-oriented programming language. We can easily create and use classes and objects in Python

## Class

Defining Classes
The following statement makes a class with no attributes attached, and in fact, it's an empty namespace object:
The name of this class is Student, and it doesn't inherit from any other class. Class names are usually capitalized, but this is only a convention, not a requirement. Everything in a class is indented, just like the code within a function, if statement, for loop, or any other block of code. The first line not indented is outside the class.
```python
class Student: 
  pass
```
We can create elements 

```python
Student.name = "Umesh" 
Student.id = 23415
```

In Python, objects are created in two steps:
Constructs an object 
__new()__
Initializes the object 
__init()__

However, it's very rare to actually need to implement __new()__ because Python constructs our objects for us. So, in most of the cases, we usually only implement the special method, __init()__.

Let's create a class that stores a string and a number:

```python
class Rectangle(object): 
    def __init__(self, w, h):
        self.width = w 		
        self.height = h 	
    def area(self):
        return self.width * self.height  	
rect = Rectangle(100,20)
print(rect.area()) 
rect.height = 30 
print(rect.area()) 
```

Note that this version is using direct attribute access for the width and height.
