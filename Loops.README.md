#Loops:<br /> 

Example 1:

```python
for i in range(5):
    print(i)
```
Example 2:

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```
Example 3:

```python
while True:
    user_input = input("Enter a number (or 'exit' to stop): ")
    if user_input.lower() == 'exit':
        break
    else:
        print(f"You entered: {user_input}")
```
Example 4:

```python
numbers = [1, 2, 3, 4, 5]
for num in numbers:
    if num % 2 == 0:
        continue
    print(num)
```
Example 5:

```python
for i in range(3):
    for j in range(2):
        print(f"({i}, {j})")
```        
Advanced Application:
```python
#Implementing a real-time data streaming application that continuously processes incoming data using loops.
Implementing a Web Crawler with Loops:

Copy code
import requests
from bs4 import BeautifulSoup

def web_crawler(url):
    for i in range(3):  # Crawl three pages
        response = requests.get(url)
        soup = BeautifulSoup(response.content, 'html.parser')
        # Extract information from the webpage here
        url = next_page_url  # Obtain the URL of the next page

# Usage
web_crawler("https://example.com")
```
