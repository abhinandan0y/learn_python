#Tuples:<br /> 

Example 1: Creating Tuples

```python
tuple1 = (1, 2, 3)
tuple2 = ('a', 'b', 'c')

print("Tuple 1:", tuple1)
print("Tuple 2:", tuple2)
```
Example 2: Tuple Unpacking

```python
coordinates = (5, 8)

x, y = coordinates
print("X Coordinate:", x)
print("Y Coordinate:", y)
```
Example 3: Immutable Nature of Tuples

```python
my_tuple = (10, 20, 30)

# This will result in an error
# my_tuple[0] = 5
```
Example 4: Tuple Concatenation

```python
tuple1 = (1, 2, 3)
tuple2 = ('a', 'b', 'c')

result = tuple1 + tuple2
print("Concatenated Tuple:", result)
```
Example 5: Tuple Methods

```python
my_tuple = (4, 2, 8, 1, 5)

max_value = max(my_tuple)
min_value = min(my_tuple)

print("Maximum Value:", max_value)
print("Minimum Value:", min_value)
```
