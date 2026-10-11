# DNA Sequence Analyzer

A beginner-friendly Python tool for analyzing DNA sequences. Built as a first step into bioinformatics, with the aim of working toward cheminformatics and machine learning for molecular design.

## Features

- [ ] **Input cleaning and validation:** uppercases input, removes whitespace, and rejects invalid characters (only A, C, G, T allowed)
- [ ] **Nucleotide counts:** number of A, C, G and T
- [ ] **GC content:** percentage of G and C bases
- [ ] **Complement and reverse complement:** the opposite DNA strand
- [ ] **Transcription:** DNA to RNA
- [ ] **Translation:** RNA/DNA to protein using the standard codon table

## Requirements

- Python 3.8 or higher
- No external libraries required

## Installation

```bash
git clone https://github.com/[your-username]/[repo-name].git
cd [repo-name]
```

## Usage

```bash
python dna_analyzer.py
```

Example input:

```
ATGCGTACGTTAGC
```

Example output:

```
Cleaned sequence:     ATGCGTACGTTAGC
Length:               14
Nucleotide counts:    A: 3, C: 3, G: 4, T: 4
GC content:           50.0%
Reverse complement:   GCTAACGTACGCAT
RNA:                  AUGCGUACGUUAGC
Protein:              [your output here]
```

*(Replace this with real output from your program.)*

## Project Structure

```
[repo-name]/
├── dna_analyzer.py    # main script
├── README.md
└── tests/             # test cases (optional)
```

## How It Works

| Function | What it does |
|---|---|
| `clean_sequence(seq)` | Normalizes and validates the input |
| `count_nucleotides(seq)` | Returns counts for each base |
| `gc_content(seq)` | Returns GC percentage |
| `reverse_complement(seq)` | Returns the reverse complement strand |
| `transcribe(seq)` | Converts DNA to RNA |
| `translate(seq)` | Converts a sequence to amino acids |

*(Adjust the function names to match your code.)*

## Testing

Results were checked against hand calculations and, where possible, against [Biopython](https://biopython.org/) (`gc_fraction`, `Seq.translate()`).

Example checks:

- `ATGC` has 50% GC content
- The reverse complement of `AAAC` is `GTTT`

## Roadmap

- [ ] Motif search (e.g. find all `ATG` positions)
- [ ] Melting temperature (Wallace rule)
- [ ] Open reading frame (ORF) finder
- [ ] FASTA file input

## Learning Goals

This project is part of my learning path:

Python → Biology → Bioinformatics → Machine Learning → Deep Learning → Molecular Modeling → Drug Repurposing → Generative Drug Design

## License

MIT License. See `LICENSE` for details.

## Author

[shashank]
[helix0931 -pixel]
