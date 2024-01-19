#Decision Making:<br />

Example 1: If Statement

```python
x = 10

if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")
    
    
```
Example 2: Elif Statement

```python
score = 75

if score >= 90:
    grade = 'A'
elif score >= 80:
    grade = 'B'
else:
    grade = 'C'

print("Grade:", grade)
```
Example 3: Ternary Operator

```python
age = 21

result = "Can vote" if age >= 18 else "Cannot vote"
print(result)
```
Example 4: Nested Decision Making

```python
x = 5
y = 10

if x > 0:
    if y > 0:
        print("Both x and y are positive")
    else:
        print("Only x is positive")
else:
    print("x is not positive")
```
Example 5: Using Logical Operators

```python
temperature = 25
humidity = 70

if temperature > 30 and humidity > 60:
    print("Too hot and humid.")
elif temperature > 30 or humidity > 60:
    print("Either too hot or too humid.")
else:
    print("Weather is comfortable.")
```
Advanced Application:
```python
#Implementing a Decision-Making Algorithm:

def make_recommendation(user_data):
    # Implement decision-making logic based on user data
    if user_data['preferences']['genre'] == 'Action':
        recommendation = 'Terminator 2'
    else:
        recommendation = 'The Shawshank Redemption'
    return recommendation

# Usage
user_data = {'preferences': {'genre': 'Action'}}
recommendation = make_recommendation(user_data)
print("Recommended Movie:", recommendation)
Result:

Recommended Movie: Terminator 2
```
