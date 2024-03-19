# learn_python

1. Classes | Objects:
```python
Example:

class DNASequence:
    def __init__(self, sequence):
        self.sequence = sequence

my_sequence = DNASequence(sequence="ATCG")
print(my_sequence.sequence)

Advanced Application:

# Creating a simulation of a gene expression system where each DNA sequence is an object with properties and methods.
```
2. Dictionary:
```python
Example:

sequence_info = {"gene_name": "TP53", "length": 1000, "type": "coding"}
print(sequence_info["gene_name"], sequence_info["length"])

Advanced Application:

# Implementing a k-mer frequency counter using a dictionary to analyze DNA sequences.
```
3. Exceptions Handling:
```python
Example:

try:
    result = calculate_entropy()
except EntropyCalculationError as e:
    print(f"Error: {e}")

# Advanced Application:

# Building a robust genome assembler with error handling to handle various types of sequencing and assembly errors.
```
4. Functions:
```python
Example:

def translate_dna_sequence(dna_sequence):
    genetic_code = {
        'ATA':'I', 'ATC':'I', 'ATT':'I', 'ATG':'M',
        'ACA':'T', 'ACC':'T', 'ACG':'T', 'ACT':'T',
        'AAC':'N', 'AAT':'N', 'AAA':'K', 'AAG':'K',
        'AGC':'S', 'AGT':'S', 'AGA':'R', 'AGG':'R',
        'CTA':'L', 'CTC':'L', 'CTG':'L', 'CTT':'L',
        'CCA':'P', 'CCC':'P', 'CCG':'P', 'CCT':'P',
        'CAC':'H', 'CAT':'H', 'CAA':'Q', 'CAG':'Q',
        'CGA':'R', 'CGC':'R', 'CGG':'R', 'CGT':'R',
        'GTA':'V', 'GTC':'V', 'GTG':'V', 'GTT':'V',
        'GCA':'A', 'GCC':'A', 'GCG':'A', 'GCT':'A',
        'GAC':'D', 'GAT':'D', 'GAA':'E', 'GAG':'E',
        'GGA':'G', 'GGC':'G', 'GGG':'G', 'GGT':'G',
        'TCA':'S', 'TCC':'S', 'TCG':'S', 'TCT':'S',
        'TTC':'F', 'TTT':'F', 'TTA':'L', 'TTG':'L',
        'TAC':'Y', 'TAT':'Y', 'TAA':'_', 'TAG':'_',
        'TGC':'C', 'TGT':'C', 'TGA':'_', 'TGG':'W',
    }
    
    protein_sequence = ""
    
    for i in range(0, len(dna_sequence)-2, 3):
        codon = dna_sequence[i:i+3]
        amino_acid = genetic_code.get(codon, 'X')  # 'X' for unknown or stop codons
        protein_sequence += amino_acid
    
    return protein_sequence

Advanced Application:

# Creating a function to predict protein secondary structure from amino acid sequence.
```
5. Loops:
```python
Example:

for i in range(5):
    print(i)

Advanced Application:

# Implementing a sequence alignment algorithm to compare DNA sequences using loops.
```
6. Multithreaded Programming:
```python
Example:

import threading

def print_numbers():
    for i in range(5):
        print(i)

thread = threading.Thread(target=print_numbers)
thread.start()

Advanced Application:

# Developing a parallel computing system for analyzing large-scale genomic datasets.
```
7. Numpy:
```python
Example:

import numpy as np

array = np.array([1, 2, 3, 4])
print(array)

import numpy as np

sequence_array = np.array(["ATCG", "GCTA", "TTAG"])
print(sequence_array)

Advanced Application:


# Using NumPy for genomic data analysis, such as SNP detection from sequencing data.
```
8. Pandas:
```python
Example:

import pandas as pd

data = {'Name': ['John', 'Alice', 'Bob'], 'Age': [25, 30, 22]}
df = pd.DataFrame(data)
print(df)

import pandas as pd

data = {'Gene': ['TP53', 'BRCA1', 'EGFR'], 'Expression': [10, 5, 8]}
df = pd.DataFrame(data)
print(df)
Advanced Application:

Analyzing and visualizing gene expression data from RNA-seq experiments using Pandas.
```
9. Strings:
```python
Example:

message = "Hello, World!"
print(message.split(","))

sequence = "ATCGATCG"
print(sequence.split("AT"))

Advanced Application:

#Developing a program to predict RNA secondary structure from nucleotide sequence.
```
10. Tuples:
```python
Example:

coordinates = (3, 4)
print(coordinates[0], coordinates[1])

coordinate = (3, 4)
print(coordinate[0], coordinate[1])

Advanced Application:

# Representing and manipulating genomic coordinates in a genome annotation database.
```
11. Decision Making:
```python
Example:

x = 10
if x > 5:
    print("Greater than 5")
else:
    print("Less than or equal to 5")

Advanced Application:

# Implementing a decision-making algorithm in a variant calling pipeline.
```
12. Environment Setup:
```
Example:

Setting up a virtual environment using venv:
bash

python -m venv myenv
source myenv/bin/activate  # On Linux/Mac

Advanced Application:

#Automating environment setup using tools like Docker for deploying applications.
# Automating environment setup using tools like ***Snakemake*** for reproducible bioinformatics pipelines.
```
13. Files I/O:
```python
Example:

with open("example.txt", "w") as file:
    file.write("Hello, File I/O!")

with open("genomic_data.txt", "r") as file:
    data = file.read()

Advanced Application:

Creating a program to read and process data from a variety of file formats.
```
14. Lists:
```python
Example:

genes = ["TP53", "BRCA1", "EGFR"]
print(genes[1])

Advanced Application:

#Implementing a queue data structure using a list for efficient data processing.
# Implementing a stack data structure to process genomic data during sequence assembly.
```
15. Modules:
```python
Example:

Creating a custom module named my_module.py with a function add_numbers:
python

# my_module.py
def add_numbers(a, b):
    return a + b

# # bioinformatics_tools.py
# def align_sequences(sequence1, sequence2):
#     pass

Advanced Application:

# Developing a modular bioinformatics toolkit for various sequence analysis tasks.
```
16. Numbers:
```python
Example:

x = 5
y = 2.5
print(x + y)
```
17. Operators:
```python
Example:

x = 10
y = 3
print(x // y)  # Integer division
```
18. Python Basic Syntax:
```python
Example:

print("Hello, Bioinformatics World!")
```

19. Variable Types:
```python
Example:

gene_name = "TP53"
gene_length = 1000
is_coding_gene = True
```

**#Knowlegde is FREE but Solution is Your's🤘🏻**

**Keep on Learning and Executing...🏃🏻** contact@:bioinformaticsfuture@gmail.com
<div style="width: 100%;">
  <img src="https://www.bioinformaticsfuture.com/images/bioinformatics_lab.png" style="width: 100%;" alt="bioinformatics_lab.png">
</div>
