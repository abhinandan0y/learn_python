# functions:

```Example 1:```
```python
def transcribe_dna_to_rna(dna_sequence):
    return dna_sequence.replace('T', 'U')

dna_sequence = "ATCGATCGATCG"
rna_sequence = transcribe_dna_to_rna(dna_sequence)
print("RNA Sequence:", rna_sequence)
```
```Example 2:```
```python
def calculate_gc_content(dna_sequence):
    gc_count = dna_sequence.count('G') + dna_sequence.count('C')
    total_bases = len(dna_sequence)
    gc_content = (gc_count / total_bases) * 100
    return gc_content

dna_sequence = "ATCGATCGATCG"
gc_content = calculate_gc_content(dna_sequence)
print("GC Content:", gc_content)
```
```Example 3:```
```python
def reverse_complement(dna_sequence):
    complement = {'A': 'T', 'T': 'A', 'C': 'G', 'G': 'C'}
    reverse_complement_sequence = ''.join(complement[base] for base in reversed(dna_sequence))
    return reverse_complement_sequence

dna_sequence = "ATCGATCGATCG"
reverse_complement_sequence = reverse_complement(dna_sequence)
print("Reverse Complement Sequence:", reverse_complement_sequence)
```
```Example 4:```
```python
def count_amino_acids(protein_sequence):
    amino_acids = {'A', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'K', 'L', 'M', 'N', 'P', 'Q', 'R', 'S', 'T', 'V', 'W', 'Y'}
    amino_acid_count = {aa: protein_sequence.count(aa) for aa in amino_acids}
    return amino_acid_count

protein_sequence = "MFTPPSPPL"
amino_acid_counts = count_amino_acids(protein_sequence)
print("Amino Acid Counts:", amino_acid_counts)
```
```Example 5:```
```python
def is_palindrome(sequence):
    return sequence == sequence[::-1]

dna_sequence = "ATCGATCGATCG"
print("Is DNA sequence a palindrome?", is_palindrome(dna_sequence))
```
Advanced Application:

Creating a function for large-scale sequence alignment:
```python
def align_sequences(sequence1, sequence2):
    # Implement sequence alignment algorithm
    alignment_score = 0
    # Assume alignment score calculation here
    return alignment_score

sequence1 = "ATCGATCGATCG"
sequence2 = "AGCTAGCTAGCT"
alignment_score = align_sequences(sequence1, sequence2)
print("Alignment Score:", alignment_score)
```
