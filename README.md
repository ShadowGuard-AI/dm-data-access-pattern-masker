![Banner](banner.png)

# dm-data-access-pattern-masker
Masks access patterns to data during masking operations. It can reorder the records before applying other masking techniques. This prevents attackers from inferring information about the data or masking algorithm through observing access timings and order. Simple to implement with random index shuffling. - Focused on Tools designed to generate or mask sensitive data with realistic-looking but meaningless values

## Install
`git clone https://github.com/ShadowGuardAI/dm-data-access-pattern-masker`

## Usage
`./dm-data-access-pattern-masker [params]`

## Parameters
- `input_file`: Path to the input CSV file
- `output_file`: Path to the output CSV file. It must not be the input file: if the output path resolves to the input file, the run refuses and exits 1 before any write.
- `--seed`: Optional seed for the random number generator (for reproducibility).
- `--header`: Specify if the input CSV file has a header row. Defaults to False.

## License
Copyright (c) ShadowGuardAI
