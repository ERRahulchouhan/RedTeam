# FuzzyAI Experiment Guide

## What this folder is for

This folder contains a cell-by-cell notebook illustrating benign mutation and robustness checks. The notebook does **not** run FuzzyAI, generate live attacks, call a model, or connect to a network.

## Methods in `experiment.ipynb`

1. Whitespace mutation
2. Case mutation
3. Punctuation mutation
4. Benign paraphrase mutation
5. Length-boundary mutation
6. Unicode normalization fixture
7. Output-format mutation
8. Batch mutation summary
9. Baseline differential
10. Score stability

Each method describes one controlled variation and its expected behavior. Run the Python cell below it to check the local fixture. These examples focus on harmless input variation.

## Interview explanation

> “I use controlled input mutations to see whether harmless changes such as spacing, case, or punctuation cause unexpected response changes. I define invariants and tolerances in advance and compare results with a baseline. This notebook demonstrates the method with fixtures, not a live fuzzing run.”

## Safe-use note

Keep mutation tests within an authorized scope, with bounded inputs and synthetic data. Consult current FuzzyAI documentation before configuring real evaluations.
