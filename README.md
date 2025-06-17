# Evolutionary CRISPR gRNA Designer

This project implements an evolutionary algorithm combined with a machine learning model to design optimized CRISPR guide RNA (gRNA) sequences predicted to have high gene-editing efficiency.

## Overview

CRISPR-Cas9 gene editing relies on guide RNAs (gRNAs) to target specific DNA sequences. Designing highly efficient gRNAs is critical for successful editing but experimentally screening candidates is costly and time-consuming.

## This repository provides a computational pipeline that:

- Trains a Random Forest classifier on experimentally labeled gRNA sequences
- Uses one-hot encoding to numerically represent gRNAs
- Evolves a population of candidate gRNAs over multiple generations via selection, crossover, and mutation
- Scores candidates using the trained model to iteratively improve sequence efficiency predictions
- Outputs a ranked list of top-performing gRNAs
## Features

- Data preprocessing for gRNA sequences
- One-hot encoding of nucleotide sequences
- Random Forest model training and evaluation
- Evolutionary algorithm with crossover and mutation operators
- Easy-to-run notebook compatible with Google Colab
## Usage

- Prepare your dataset with gRNA sequences and activity labels.
- Train the Random Forest model using the provided scripts.
- Run the evolutionary algorithm to generate optimized gRNAs.
- Analyze and validate the top candidate sequences.
## Requirements

- Python 3.x
- NumPy
- Pandas
- scikit-learn
## How to Run

### Clone the repository:
```git clone https://github.com/yourusername/crispr-evolution.git ```
```cd crispr-evolution```
### Install dependencies:
```pip install numpy pandas scikit-learn```
Run the main notebook or script in Google Colab or locally.
## License

MIT License
