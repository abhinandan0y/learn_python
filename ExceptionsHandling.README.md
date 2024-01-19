#Exceptions Handling:<br /> 

Example 1:

```python

try:
    result = 10 / 0
except ZeroDivisionError as e:
    print(f"Error: {e}")
```
Example 2:

```python

try:
    num = int("abc")
except ValueError as e:
    print(f"Error: {e}")
```
Example 3:

```python

try:
    file = open("nonexistent.txt", "r")
except FileNotFoundError as e:
    print(f"Error: {e}")
```
Example 4:

```python

try:
    data = [1, 2, 3]
    print(data[4])
except IndexError as e:
    print(f"Error: {e}")
```
Example 5:

```python

try:
    x = int(input("Enter a number: "))
except ValueError:
    print("Invalid input. Please enter a valid number.")
else:
    print(f"You entered: {x}")
```
Advanced Application:

``````python
#Building a Robust Web Scraper with Error Handling:

import requests
from bs4 import BeautifulSoup

url = "https://```
Example.com"

try:
    response = requests.get(url)
    response.raise_for_status()  # Check for HTTP errors
    soup = BeautifulSoup(response.content, 'html.parser')
    # Parsing logic here

except requests.RequestException as e:
    print(f"Error: {e}")
except Exception as e:
    print(f"Unexpected error: {e}")
```
