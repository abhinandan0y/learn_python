#Variable Types:<br /> 
Python has several variable types, including integers, floats, strings, lists, tuples, etc.
```python
Example:

# Variable types
integer_var = 5
float_var = 2.5
string_var = "Hello, Python!"

print("Integer Variable:", integer_var)
print("Float Variable:", float_var)
print("String Variable:", string_var)
```
Advanced Application Example:
```python
Consider a scenario where you want to create a module for handling mathematical operations on complex numbers:

# ComplexMath.py

import cmath

def add_complex(a, b):
    return a + b

def multiply_complex(a, b):
    return a * b

# Advanced Application: Calculate the magnitude of a complex number
def magnitude_complex(z):
    return abs(z)

# Main script
import ComplexMath

complex_num_1 = 3 + 4j
complex_num_2 = 1 - 2j

result_sum = ComplexMath.add_complex(complex_num_1, complex_num_2)
result_product = ComplexMath.multiply_complex(complex_num_1, complex_num_2)
result_magnitude = ComplexMath.magnitude_complex(complex_num_1)

print("Sum of Complex Numbers:", result_sum)
print("Product of Complex Numbers:", result_product)
print("Magnitude of Complex Number:", result_magnitude)
```
