#Operators:<br /> 
1. Arithmetic Operators:
```python
# Arithmetic Operators
a = 10
b = 3

addition = a + b
subtraction = a - b
multiplication = a * b
division = a / b
remainder = a % b
exponentiation = a ** b

print("Addition:", addition)
print("Subtraction:", subtraction)
print("Multiplication:", multiplication)
print("Division:", division)
print("Remainder:", remainder)
print("Exponentiation:", exponentiation)
Output:

Addition: 13
Subtraction: 7
Multiplication: 30
Division: 3.3333333333333335
Remainder: 1
Exponentiation: 1000
```
2. Comparison Operators:
```python
# Comparison Operators
x = 5
y = 10

equal = x == y
not_equal = x != y
greater_than = x > y
less_than = x < y
greater_than_equal = x >= y
less_than_equal = x <= y

print("Equal:", equal)
print("Not Equal:", not_equal)
print("Greater Than:", greater_than)
print("Less Than:", less_than)
print("Greater Than or Equal:", greater_than_equal)
print("Less Than or Equal:", less_than_equal)
Output:

Equal: False
Not Equal: True
Greater Than: False
Less Than: True
Greater Than or Equal: False
Less Than or Equal: True
```
3. Logical Operators:
```python
# Logical Operators
p = True
q = False

and_result = p and q
or_result = p or q
not_result_p = not p
not_result_q = not q

print("AND Result:", and_result)
print("OR Result:", or_result)
print("NOT Result (p):", not_result_p)
print("NOT Result (q):", not_result_q)
Output:

AND Result: False
OR Result: True
NOT Result (p): False
NOT Result (q): True
```
4. Assignment Operators:
```python
# Assignment Operators
x = 5

x += 3
y = x * 2
z = 2 ** x

print("Updated x (x += 3):", x)
print("y (y = x * 2):", y)
print("z (z = 2 ** x):", z)
Output:

Updated x (x += 3): 8
y (y = x * 2): 16
z (z = 2 ** x): 256
```
5. Identity Operators:
```python
# Identity Operators
a = [1, 2, 3]
b = [1, 2, 3]
c = a

is_result = a is b
is_not_result = a is not b
is_c_result = a is c

print("is Result:", is_result)
print("is not Result:", is_not_result)
print("is c Result:", is_c_result)
Output:

```python
is Result: False
is not Result: True
is c Result: True
```
6. Membership Operators:
```python
# Membership Operators
sample_list = [1, 2, 3, 4, 5]

in_result = 3 in sample_list
not_in_result = 6 not in sample_list

print("In Result:", in_result)
print("Not In Result:", not_in_result)
Output:

In Result: True
Not In Result: True
```
