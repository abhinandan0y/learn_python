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
# Advanced Application: Bioinformatics Data Processing Program

# BioinformaticsFileProcessor.py

import csv
import json
import xml.etree.ElementTree as ET

class BioinformaticsFileProcessor:
    def __init__(self, file_path):
        self.file_path = file_path

    def read_fasta(self):
        sequences = {}
        with open(self.file_path, 'r') as file:
            current_sequence_id = ''
            current_sequence = ''
            for line in file:
                if line.startswith('>'):
                    if current_sequence:
                        sequences[current_sequence_id] = current_sequence
                        current_sequence = ''
                    current_sequence_id = line.strip()[1:]
                else:
                    current_sequence += line.strip()
            if current_sequence:
                sequences[current_sequence_id] = current_sequence
        return sequences

    def read_genbank(self):
        sequences = {}
        with open(self.file_path, 'r') as file:
            for line in file:
                if line.startswith('LOCUS'):
                    current_sequence_id = line.split()[1]
                    current_sequence = ''
                elif line.startswith('ORIGIN'):
                    current_sequence = ''
                elif line.startswith('//'):
                    sequences[current_sequence_id] = current_sequence
                else:
                    current_sequence += line.strip().upper().replace(' ', '')
        return sequences

    def read_phylip(self):
        sequences = {}
        with open(self.file_path, 'r') as file:
            lines = file.readlines()
            num_sequences = int(lines[0].strip().split()[0])
            for i in range(1, len(lines)):
                current_line = lines[i].strip().split()
                sequences[current_line[0]] = current_line[1]
        return sequences

# Main script
file_path_fasta = 'sequences.fasta'
file_path_genbank = 'sequences.gb'
file_path_phylip = 'sequences.phy'

fasta_sequences = BioinformaticsFileProcessor(file_path_fasta).read_fasta()
genbank_sequences = BioinformaticsFileProcessor(file_path_genbank).read_genbank()
phylip_sequences = BioinformaticsFileProcessor(file_path_phylip).read_phylip()

# Example usage of processed data
print("FASTA Sequences:")
print(fasta_sequences)

print("\nGenBank Sequences:")
print(genbank_sequences)

print("\nPhylip Sequences:")
print(phylip_sequences)
```



