# learn_python

1. Classes | Objects:
```
Example:

python
Copy code
class Car:
    def __init__(self, brand, model):
        self.brand = brand
        self.model = model

my_car = Car(brand="Toyota", model="Camry")
print(my_car.brand, my_car.model)
Advanced Application:

Creating a simulation of a car rental system where each car is an object with properties and methods.
```
2. Dictionary:
```
Example:

python
Copy code
student = {"name": "John", "age": 20, "grade": "A"}
print(student["name"], student["age"])
Advanced Application:

Implementing a word frequency counter using a dictionary to analyze text data.
```
3. Exceptions Handling:
```
Example:

python
Copy code
try:
    result = 10 / 0
except ZeroDivisionError as e:
    print(f"Error: {e}")
Advanced Application:

Building a robust web scraper with error handling to handle various types of network and parsing errors.
```
4. Functions:
```
Example:

python
Copy code
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))
Advanced Application:

Creating a function to process and analyze large datasets efficiently.
```
5. Loops:
```
Example:

python
Copy code
for i in range(5):
    print(i)
Advanced Application:

Implementing a web crawler to extract information from multiple pages on a website using loops.
```
6. Multithreaded Programming:
```
Example:

python
Copy code
import threading

def print_numbers():
    for i in range(5):
        print(i)

thread = threading.Thread(target=print_numbers)
thread.start()
Advanced Application:

Developing a parallel processing system for handling large-scale data analysis tasks.
```
7. Numpy:
```
Example:

python
Copy code
import numpy as np

array = np.array([1, 2, 3, 4])
print(array)
Advanced Application:

Using NumPy for numerical operations in machine learning algorithms, such as matrix multiplication.
```
8. Pandas:
```
Example:

python
Copy code
import pandas as pd

data = {'Name': ['John', 'Alice', 'Bob'], 'Age': [25, 30, 22]}
df = pd.DataFrame(data)
print(df)
Advanced Application:

Analyzing and visualizing large datasets from a CSV file using Pandas.
```
9. Strings:
```
Example:

python
Copy code
message = "Hello, World!"
print(message.split(","))
Advanced Application:

Developing a text-based natural language processing application.
```
10. Tuples:
```
Example:

python
Copy code
coordinates = (3, 4)
print(coordinates[0], coordinates[1])
Advanced Application:

Representing and manipulating coordinates in a geographical information system (GIS).
```
11. Decision Making:
```
Example:

python
Copy code
x = 10
if x > 5:
    print("Greater than 5")
else:
    print("Less than or equal to 5")
Advanced Application:

Implementing a decision-making algorithm in a recommendation system.
```
12. Environment Setup:
```
Example:

Setting up a virtual environment using venv:
bash
Copy code
python -m venv myenv
source myenv/bin/activate  # On Linux/Mac
Advanced Application:

Automating environment setup using tools like Docker for deploying applications.

```
13. Files I/O:
```
Example:

python
Copy code
with open("example.txt", "w") as file:
    file.write("Hello, File I/O!")
Advanced Application:

Creating a program to read and process data from a variety of file formats.
```
14. Lists:
```
Example:

python
Copy code
fruits = ["apple", "banana", "orange"]
print(fruits[1])
Advanced Application:

Implementing a queue data structure using a list for efficient data processing.
```
15. Modules:
```
Example:

Creating a custom module named my_module.py with a function add_numbers:
python
Copy code
# my_module.py
def add_numbers(a, b):
    return a + b
Advanced Application:

Developing a modular architecture for a complex software system.
```
16. Numbers:
```
Example:

python
Copy code
x = 5
y = 2.5
print(x + y)
Advanced Application:

Implementing numerical simulations or scientific computing using advanced mathematical operations.
```
17. Operators:
```
Example:

python
Copy code
x = 10
y = 3
print(x // y)  # Integer division
Advanced Application:

Overloading operators for custom classes to define specific behavior.
```
18. Python Basic Syntax:
```
Example:

python
Copy code
print("Hello, World!")
Advanced Application:

Building a code formatter or linter to enforce coding standards.
```

20. Variable Types:
```
Example:

python
Copy code
name = "John"
age = 25
is_student = True
Advanced Application:

Implementing dynamic typing in a scripting language interpreter or developing a type-checking tool.
```
