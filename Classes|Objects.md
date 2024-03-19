# bioinformatics_classes_objects:

class DNASequence:
    def __init__(self, sequence_id, sequence):
        self.sequence_id = sequence_id
        self.sequence = sequence

sequence1 = DNASequence("Seq1", "ATCGATCG")
print(sequence1.sequence_id, sequence1.sequence)

class Protein:
    def __init__(self, name, sequence):
        self.name = name
        self.sequence = sequence

protein1 = Protein("Hemoglobin", "MFTPPSPPL")
print(protein1.name, protein1.sequence)

class Gene:
    def __init__(self, symbol, sequence):
        self.symbol = symbol
        self.sequence = sequence

gene1 = Gene("BRCA1", "ATCGTATG")
print(gene1.symbol, gene1.sequence)

# Advanced Application:

# Creating a simulation of a genetic engineering lab where each DNA sequence, protein, or gene is represented as an object with properties and methods.

# bioinformatics_advanced_application:

class SequenceAnalysis:
    def __init__(self, sequence):
        self.sequence = sequence

    def calculate_gc_content(self):
        gc_count = self.sequence.count('G') + self.sequence.count('C')
        total_bases = len(self.sequence)
        gc_content = (gc_count / total_bases) * 100
        return gc_content

dna_sequence = SequenceAnalysis("ATCGATCGATCG")
print("GC Content:", dna_sequence.calculate_gc_content())

# Advanced Application:

# Developing a bioinformatics toolkit for sequence analysis with methods to calculate GC content, perform sequence alignment, and predict protein structure.

