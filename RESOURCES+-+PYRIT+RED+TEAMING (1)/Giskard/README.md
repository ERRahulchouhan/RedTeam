# Giskard Experiment Guide

## What this folder is for

This folder contains a cell-by-cell notebook of safe, fictional AI evaluation examples. It illustrates dataset, source-grounding, slice, and regression checks. It does **not** run Giskard or evaluate a live model or RAG system.

## Methods in `experiment.ipynb`

1. Synthetic dataset validation
2. RAG source-grounding check
3. Hallucination spot check
4. Sensitive-data check
5. Fairness slice parity fixture
6. Response-quality threshold
7. Regression scan fixture
8. Format validation
9. Robustness slice
10. Action policy slice

Read each Markdown explanation, then run its separate Python check. The checks use fictional data and demonstrate assertions, not product-specific APIs.

## Interview explanation

> “I evaluate AI systems with controlled datasets and measurable checks for grounding, privacy, output quality, robustness, and regression. I compare relevant slices carefully and document limitations. This notebook demonstrates fixture checks, not a Giskard scan or fairness certification.”

## Safe-use note

Use synthetic or approved data, especially for privacy and slice testing. Consult current Giskard documentation before connecting a real model or retrieval pipeline.
