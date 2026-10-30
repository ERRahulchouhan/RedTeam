# PyRIT Experiment Guide

## What this folder is for

This folder contains a cell-by-cell notebook of safe, fictional evaluation examples associated with PyRIT-style red-team workflows. The notebook does **not** import or execute PyRIT, contact a model, or make network requests.

## Methods in `experiment.ipynb`

1. Orchestrated conversation replay
2. Objective-based scorer calibration
3. Multi-turn state check
4. Synthetic canary leakage check
5. Batch dataset evaluation
6. Conversation regression replay
7. Refusal scorer check
8. Mock tool-policy orchestration
9. Output-format scoring
10. Grounded-response evaluator

Each method has an explanation cell followed by an independent Python assertion. Read the goal and expected result, then run its code cell. `PASS` means only that the sample fixture satisfied the assertion.

## Interview explanation

> “I structure an authorized AI red-team evaluation as reproducible conversations with explicit objectives and scoring criteria. I use synthetic cases, inspect the evidence, and turn confirmed behavior into regression checks. This notebook illustrates the approach; it is not a live PyRIT run.”

## Safe-use note

Only test systems you are authorized to assess. Use synthetic data. Consult the current PyRIT documentation before building a real integration. A passing fixture is not a security certification.
