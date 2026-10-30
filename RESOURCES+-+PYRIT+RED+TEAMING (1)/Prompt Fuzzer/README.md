# Prompt Fuzzer Experiment Guide

## What this folder is for

This folder contains a cell-by-cell notebook showing controlled, benign prompt-variation checks. It does **not** run a fuzzer, call a model, or send prompts to an external service.

## Methods in `experiment.ipynb`

1. Whitespace-only mutation
2. Capitalization mutation
3. Punctuation mutation
4. Benign paraphrase sweep
5. Length-boundary sweep
6. Unicode-form sweep
7. Schema-preservation sweep
8. Batch pass-rate report
9. Invariant sweep
10. Score-variance sweep

Each explanation states what varies and what should remain stable. Run the following Python cell to check the fictional observation and its assertion.

## Interview explanation

> “I vary one benign input property at a time, define the expected invariant, and compare normalized outputs. This helps make robustness checks measurable and reproducible. The notebook uses safe fixtures only and does not demonstrate a live prompt-fuzzer run.”

## Safe-use note

Use bounded, harmless test cases against authorized systems. Follow the selected fuzzer's current documentation for real integrations and avoid sensitive data.
