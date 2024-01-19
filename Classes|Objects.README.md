#Classes | Objects:
\n
Example 1:
```
class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = agedog1 = Dog("Buddy", 3)
print(dog1.name, dog1.age)
```
Example 2:
```
class Circle:
    def __init__(self, radius):
        self.radius = radius    def area(self):
        return 3.14 * self.radius ** 2circle1 = Circle(5)
print("Area of Circle:", circle1.area())
```
Example 3:
```
class Student:
    def __init__(self, name, grade):
        self.name = name
        self.grade = gradestudent1 = Student("Alice", "A")
print(f"{student1.name} scored {student1.grade} grade.")
```
Example 4:
```
class Book:
    def __init__(self, title, author):
        self.title = title
        self.author = authorbook1 = Book(" Crash Course", "Eric Matthes")
print(f"{book1.title} by {book1.author}")
```
Example 5:
```
class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = modelcar1 = Car("Toyota", "Camry")
print(f"Car: {car1.brand} {car1.model}")
```
#### Advanced Application:
Creating a Simulation of a Car Rental System:
```
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

Copy code
Renting Toyota Camry
Renting Honda Accord
Returning Toyota Camry
```
