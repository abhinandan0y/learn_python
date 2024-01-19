#File I/O:<br /> 

Example 1: Reading from a Text File

```python
with open('Example.txt', 'r') as file:
    content = file.read()
    print("File Content:", content)
```
Example 2: Writing to a Text File

```python
with open('output.txt', 'w') as file:
    file.write("Hello, File I/O!")
```
Example 3: Reading CSV File using Pandas

```python
import pandas as pd

data = pd.read_csv('data.csv')
print("CSV Data:")
print(data)
```
Example 4: Writing to CSV File using Pandas

```python
import pandas as pd

data = {'Name': ['Alice', 'Bob', 'Charlie'], 'Age': [25, 30, 22]}
df = pd.DataFrame(data)

df.to_csv('output.csv', index=False)
```
Example 5: Pickle Serialization

```python
import pickle

data = {'Name': 'Alice', 'Age': 25}

with open('data.pkl', 'wb') as file:
    pickle.dump(data, file)

with open('data.pkl', 'rb') as file:
    loaded_data = pickle.load(file)
    print("Loaded Data:", loaded_data)
```
Advanced Application:
```python
#Developing a data pipeline that reads streaming data from sensors, processes it, and stores it in a distributed file system for further analysis.
#Advanced Application: Data Processing Program

# FileProcessor.py

import csv
import json
import xml.etree.ElementTree as ET

class FileProcessor:
    def __init__(self, file_path):
        self.file_path = file_path

    def read_csv(self):
        with open(self.file_path, 'r') as file:
            reader = csv.reader(file)
            data = [row for row in reader]
        return data

    def read_json(self):
        with open(self.file_path, 'r') as file:
            data = json.load(file)
        return data

    def read_xml(self):
        tree = ET.parse(self.file_path)
        root = tree.getroot()
        data = []

        for element in root:
            record = {}
            for child in element:
                record[child.tag] = child.text
            data.append(record)

        return data

# Main script
file_path_csv = 'data.csv'
file_path_json = 'data.json'
file_path_xml = 'data.xml'

csv_data = FileProcessor(file_path_csv).read_csv()
json_data = FileProcessor(file_path_json).read_json()
xml_data = FileProcessor(file_path_xml).read_xml()

# Example usage of processed data
print("CSV Data:")
print(csv_data)

print("\nJSON Data:")
print(json_data)

print("\nXML Data:")
print(xml_data)
```
