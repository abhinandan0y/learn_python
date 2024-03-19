# decision_making:

```Example 1: If Statement```
```python
mutation_count = 20

if mutation_count > 10:
    print("High mutation count detected.")
else:
    print("Mutation count within normal range.")
```
```Example 2: Elif Statement```
```python
gene_expression = 150

if gene_expression >= 200:
    expression_level = 'High'
elif gene_expression >= 100:
    expression_level = 'Moderate'
else:
    expression_level = 'Low'

print("Expression Level:", expression_level)
```
```Example 3: Ternary Operator```
```python
mutation_type = 'SNP'

result = "High impact" if mutation_type == 'SNP' else "Low impact"
print("Mutation Impact:", result)
```
```Example 4: Nested Decision Making```
```python
dna_length = 500
gc_content = 60

if dna_length > 100:
    if gc_content > 50:
        print("High GC content in long DNA sequence.")
    else:
        print("Low GC content in long DNA sequence.")
else:
    print("DNA sequence length not sufficient for analysis.")
```
```Example 5: Using Logical Operators```
```python
temperature = 25
humidity = 70

if temperature > 30 and humidity > 60:
    print("High temperature and humidity detected.")
elif temperature > 30 or humidity > 60:
    print("Either high temperature or humidity detected.")
else:
    print("Temperature and humidity within normal range.")

Advanced Application:

```Implementing a Decision-Making Algorithm:```
```python
def predict_variant_effect(variant_data):
    # Implement decision-making logic based on variant data
    if variant_data['impact'] == 'HIGH':
        effect = 'Pathogenic'
    else:
        effect = 'Benign'
    return effect

Usage
variant_data = {'impact': 'HIGH'}
effect_prediction = predict_variant_effect(variant_data)
print("Predicted Variant Effect:", effect_prediction)
```
