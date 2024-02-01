#
Using a for loop:
```python
numbers = [1, 2, 3, 4, 5]
squared_numbers = []

for num in numbers:
    squared_numbers.append(num ** 2)

print(squared_numbers)
```
Using list comprehension:
```python
numbers = [1, 2, 3, 4, 5]
squared_numbers = [num ** 2 for num in numbers]

print(squared_numbers)
```
Using the map() function with a lambda function:

```python
numbers = [1, 2, 3, 4, 5]
squared_numbers = list(map(lambda num: num ** 2, numbers))

print(squared_numbers)
```
