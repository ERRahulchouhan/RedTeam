# promptfoo Experiment Guide

## What this folder is for

This folder contains a cell-by-cell notebook demonstrating evaluation concepts commonly used in prompt and model testing. The notebook does **not** invoke promptfoo, a provider, a live model, or an external service.

## Methods in `experiment.ipynb`

1. Assertion-based evaluation
2. Prompt-variable matrix
3. Provider comparison fixture
4. Rubric threshold
5. JSON schema assertion
6. Golden regression case
7. Refusal expectation
8. Groundedness assertion
9. Benign robustness matrix
10. Tool-use assertion

Read each test explanation and run its corresponding code cell. Assertions make the pass criteria explicit; a `PASS` applies only to the fixture shown.

## Interview explanation

> “I make prompt evaluations repeatable with explicit assertions, a small input matrix, and regression cases. I compare outputs against defined criteria rather than relying on a single subjective example. This notebook demonstrates the test logic but is not a promptfoo execution.”

## Safe-use note

For a real evaluation, follow promptfoo's current documentation, configure only approved providers and targets, and avoid entering real secrets or personal data into test prompts.
