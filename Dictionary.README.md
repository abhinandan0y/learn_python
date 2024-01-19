#Dictionary::<br /> 

Example 1:

```python
student = {"name": "John", "age": 20, "grade": "A"}
print(student["name"], student["age"])
```
Example 2:

```python
employee = {"id": 101, "name": "Alice", "position": "Software Engineer"}
print(f"{employee['name']} ({employee['position']}) - Employee ID: {employee['id']}")
```
Example 3:

```python
country_capitals = {"USA": "Washington D.C.", "France": "Paris", "India": "New Delhi"}
print(country_capitals["France"])
```
Example 4:

```python
fruit_prices = {"apple": 1.00, "banana": 0.75, "orange": 1.20}
fruit_prices["grape"] = 2.50  # Adding a new entry
print(fruit_prices)
```
Example 5:

```python
car_info = dict(make="Toyota", model="Camry", year=2022)
print(car_info)
```

Advanced Application:
```python
#Implementing a Word Frequency Counter:

text = "This is a sample text. ```python is powerful. ```python is versatile."

word_frequency = {}
words = text.split()

for word in words:
    word = word.lower()
    if word.isalpha():
        if word in word_frequency:
            word_frequency[word] += 1
        else:
            word_frequency[word] = 1

print("Word Frequency:", word_frequency)
Result:

css
Copy code
Word Frequency: {'this': 1, 'is': 2, 'a': 1, 'sample': 1, 'text': 1, '```python': 2, 'powerful': 1, 'versatile': 1}
```
