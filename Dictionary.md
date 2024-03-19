# bioinformatics_dictionary:

```Example 1:```
```python
sequence_info = {"gene_name": "TP53", "length": 1000, "type": "coding"}
print(sequence_info["gene_name"], sequence_info["length"])
```
```Example 2:```
```python
sequence_properties = {"id": "SEQ001", "sequence": "ATCGATCG", "source": "GenBank"}
print(f"Sequence ID: {sequence_properties['id']}, Source: {sequence_properties['source']}")
```
```Example 3:```
```python
genome_assemblies = {"GRCh38": "Human", "GRCm39": "Mouse", "CanFam4": "Dog"}
print(genome_assemblies["GRCh38"])
```
```Example 4:```
```python
sequence_counts = {"A": 25, "T": 30, "C": 20, "G": 25}
sequence_counts["N"] = 10  # Adding a new entry
print(sequence_counts)
```
```Example 5:```
```python
bioinformatics_tools = dict(aligner="BLAST", simulator="SimSeq", assembler="SPAdes")
print(bioinformatics_tools)
```
Advanced Application:

```Implementing a k-mer frequency counter:```
```python
dna_sequence = "ATCGATCGATCG"
kmer_length = 3

kmer_frequency = {}
for i in range(len(dna_sequence) - kmer_length + 1):
    kmer = dna_sequence[i:i + kmer_length]
    if kmer in kmer_frequency:
        kmer_frequency[kmer] += 1
    else:
        kmer_frequency[kmer] = 1

print("K-mer Frequency:", kmer_frequency)
```
