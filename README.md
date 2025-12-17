# Computational Theory

A Jupyter notebook implementing SHA-256 cryptographic hash algorithm from scratch, demonstrating core concepts in computational theory.

## Overview

This repository contains solutions to computational theory problems that build up to a complete SHA-256 implementation:

- **Problem 1**: Bitwise operations used in SHA-256 (Parity, Choice, Majority, Sigma functions)
- **Problem 2**: Deriving SHA-256 round constants from prime number cube roots
- **Problem 3**: Message padding according to the Secure Hash Standard (FIPS 180-4)
- **Problem 4**: Complete SHA-256 hash function implementation
- **Problem 5**: Password cracking using dictionary attacks with the SHA-256 implementation

## Requirements

- Python 3.12+
- NumPy

## Getting Started

### Using GitHub Codespaces

1. Click the **Code** button on GitHub and select **Open with Codespaces**
2. The dev container will automatically set up the environment
3. Open `problems.ipynb` in VS Code's Jupyter extension


## Running the Code

Open `problems.ipynb` and run the cells sequentially. Each problem section contains:

- Markdown explanations of the concepts
- Python implementations
- Test functions that validate the code

The notebook is designed to be run from top to bottom, as later problems depend on functions defined in earlier ones.

## Project Structure

```
computational_theory/
├── .devcontainer/       # Dev container configuration for Codespaces
│   ├── devcontainer.json
│   └── Dockerfile
├── problems.ipynb       # Main notebook with all implementations
└── README.md
```
