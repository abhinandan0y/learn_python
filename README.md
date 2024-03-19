# learn_python

1. Classes | Objects:
```python
Example:

class DNASequence:
    def __init__(self, sequence):
        self.sequence = sequence

my_sequence = DNASequence(sequence="ATCG")
print(my_sequence.sequence)

Advanced Application:

Creating a simulation of a car rental system where each car is an object with properties and methods.
```
2. Dictionary:
```python
Example:


sequence_info = {"gene_name": "TP53", "length": 1000, "type": "coding"}
print(sequence_info["gene_name"], sequence_info["length"])

Advanced Application:

Implementing a word frequency counter using a dictionary to analyze text data.
```
3. Exceptions Handling:
```python
Example:

try:
    result = 10 / 0
except ZeroDivisionError as e:
    print(f"Error: {e}")

Advanced Application:

Building a robust web scraper with error handling to handle various types of network and parsing errors.
```
4. Functions:
```python
Example:

def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))

Advanced Application:

Creating a function to process and analyze large datasets efficiently.
```
5. Loops:
```python
Example:

for i in range(5):
    print(i)

Advanced Application:

Implementing a web crawler to extract information from multiple pages on a website using loops.
```
6. Multithreaded Programming:
```python
Example:

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
```python
Example:

import numpy as np

array = np.array([1, 2, 3, 4])
print(array)

import numpy as np

sequence_array = np.array(["ATCG", "GCTA", "TTAG"])
print(sequence_array)

Advanced Application:

Using NumPy for numerical operations in machine learning algorithms, such as matrix multiplication.
```
8. Pandas:
```python
Example:

import pandas as pd

data = {'Name': ['John', 'Alice', 'Bob'], 'Age': [25, 30, 22]}
df = pd.DataFrame(data)
print(df)

import pandas as pd

data = {'Gene': ['TP53', 'BRCA1', 'EGFR'], 'Expression': [10, 5, 8]}
df = pd.DataFrame(data)
print(df)
Advanced Application:

Analyzing and visualizing large datasets from a CSV file using Pandas.
```
9. Strings:
```python
Example:

message = "Hello, World!"
print(message.split(","))

sequence = "ATCGATCG"
print(sequence.split("AT"))

Advanced Application:

Developing a text-based natural language processing application.
```
10. Tuples:
```python
Example:

coordinates = (3, 4)
print(coordinates[0], coordinates[1])

coordinate = (3, 4)
print(coordinate[0], coordinate[1])

Advanced Application:

Representing and manipulating coordinates in a geographical information system (GIS).
```
11. Decision Making:
```python
Example:

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

python -m venv myenv
source myenv/bin/activate  # On Linux/Mac

Advanced Application:

Automating environment setup using tools like Docker for deploying applications.

```
13. Files I/O:
```python
Example:

with open("example.txt", "w") as file:
    file.write("Hello, File I/O!")

with open("genomic_data.txt", "r") as file:
    data = file.read()

Advanced Application:

Creating a program to read and process data from a variety of file formats.
```
14. Lists:
```python
Example:

genes = ["TP53", "BRCA1", "EGFR"]
print(genes[1])

Advanced Application:

Implementing a queue data structure using a list for efficient data processing.
```
15. Modules:
```python
Example:

Creating a custom module named my_module.py with a function add_numbers:
python

# my_module.py
def add_numbers(a, b):
    return a + b

# # bioinformatics_tools.py
# def align_sequences(sequence1, sequence2):
#     pass

Advanced Application:

Developing a modular architecture for a complex software system.
```
16. Numbers:
```python
Example:

x = 5
y = 2.5
print(x + y)

Advanced Application:

Implementing numerical simulations or scientific computing using advanced mathematical operations.
```
17. Operators:
```python
Example:

x = 10
y = 3
print(x // y)  # Integer division

Advanced Application:

Overloading operators for custom classes to define specific behavior.
```
18. Python Basic Syntax:
```python
Example:

print("Hello, Bioinformatics World!")

Advanced Application:

Building a code formatter or linter to enforce coding standards.
```

19. Variable Types:
```python
Example:

gene_name = "TP53"
gene_length = 1000
is_coding_gene = True

Advanced Application:

Implementing dynamic typing in a scripting language interpreter or developing a type-checking tool.
```

**#Knowlegde is FREE but Solution is Your's🤘🏻**

**Keep on Learning and Executing...🏃🏻** contact@:bioinformaticsfuture@gmail.com
<div style="width: 100%;">
  <img src="https://www.bioinformaticsfuture.com/images/bioinformatics_lab.png" style="width: 100%;" alt="bioinformatics_lab.png">
</div>
