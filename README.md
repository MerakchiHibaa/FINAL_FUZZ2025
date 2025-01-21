This repository contains the implementation of the Relative Fuzzy Temporal Hamming (RFTH) similarity measure. RFTH is designed to compare sequences of varying lengths while simultaneously capturing their semantic and temporal similarities. It leverages fuzzy logic for robust performance and has diverse applications, including human mobility analysis, patient records, and weather data comparison.

## Features
- Handles sequences of varying lengths.
- Fuzzy logic for adaptable similarity computation.
- Applications: Human mobility, patient records, weather data, etc.

## Installation
1. Clone this repository:
    ```bash
    git clone https://github.com/MerakchiHibaa/FINAL_FUZZ2025.git
    ```
2. Install dependencies
3. Download the ontology
4. Define sequences
```
# Example : 
S1 = Temporal_seq(['2', '4', '5'], [60, 240, 120])
S2 = Temporal_seq(['1', '4', '1'], [30, 300, 30])
```
6. Compute FTH distance using FTH_relative_fuzz
```
# Example : 
distance = FTH_relative_fuzz(S1, S2, f=cost_delta_fth)
print(f"RFTH Distance: {distance}")
```
8. Compute the Sim_Delta based on the FTH distance using the similarity_fth function
9. Calculate the t-length comparability index using the IC function
10. Calculate the agregated value of the t-length comparabity index and Sim_Delta with the product, minimum, or Lukasiewicz T-Norm
