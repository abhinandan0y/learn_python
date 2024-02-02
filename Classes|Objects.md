#Classes | Objects:<br /> 

Example 1:

```python
class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age

dog1 = Dog("Buddy", 3)
print(dog1.name, dog1.age)
```
Example 2:
```python

class Circle:
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return 3.14 * self.radius ** 2

circle1 = Circle(5)
print("Area of Circle:", circle1.area())
```
Example 3:
```python

class Student:
    def __init__(self, name, grade):
        self.name = name
        self.grade = grade

student1 = Student("Alice", "A")
print(f"{student1.name} scored {student1.grade} grade.")
```
Example 4:
```python

class Book:
    def __init__(self, title, author):
        self.title = title
        self.author = author

book1 = Book("Python Crash Course", "Eric Matthes")
print(f"{book1.title} by {book1.author}")
```
Example 5:
```python

class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

car1 = Car("Toyota", "Camry")
print(f"Car: {car1.brand} {car1.model}")
```
#### Advanced Application:

```python
#Creating a Simulation of a Car Rental System:
class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model
        self.available = True

    def rent(self):
        if self.available:
            print(f"Renting {self.brand} {self.model}")
            self.available = False
        else:
            print("Car not available for rent")

    def return_car(self):
        print(f"Returning {self.brand} {self.model}")
        self.available = True

# Usage
car1 = Car("Toyota", "Camry")
car2 = Car("Honda", "Accord")

car1.rent()
car2.rent()

car1.return_car()
Result:

Renting Toyota Camry
Renting Honda Accord
Returning Toyota Camry
```
