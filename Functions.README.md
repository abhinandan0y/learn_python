#Functions:<br /> 

Example 1:

```python
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))
```
Example 2:

```python
def add_numbers(a, b):
    return a + b

result = add_numbers(3, 5)
print("Sum:", result)
```
Example 3:

```python
def square(number):
    return number ** 2

print("Square of 4:", square(4))
```
Example 4:

```python
def find_max(nums):
    return max(nums)

numbers = [2, 8, 1, 6, 4]
print("Maximum:", find_max(numbers))
```
Example 5:

```python
def is_even(num):
    return num % 2 == 0

print("Is 7 even?", is_even(7))
```
Advanced Application:
```python
#Creating a machine learning model evaluation function that takes predicted and actual values to calculate performance metrics.
Creating a Function for Large Dataset Analysis:
```python

def process_large_dataset(data):
    # Perform complex analysis on the dataset
    result = sum(data)
    return result

# Usage
large_data = [i for i in range(1, 1000001)]
result = process_large_dataset(large_data)
print("Result:", result)
Result:

makefile
Copy code
Result: 500000500000
```

```
