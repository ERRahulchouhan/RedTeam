# garak Experiment Guide

## What this folder is for

This folder contains a cell-by-cell notebook of safe, fictional probe-style evaluation examples. The notebook does **not** run garak, call a model, or connect to a network.

## Methods in `experiment.ipynb`

1. Probe-style harmless baseline
2. Canary exposure probe
3. Prompt-variation probe
4. Refusal-category probe
5. Unsupported-claim probe
6. Output-shape probe
7. Batch probe set
8. Score-threshold probe
9. Regression probe
10. Mock permission probe

Each method explains its goal and expected result before a separate Python check. Run the cells individually. A `PASS` validates the local example only.

## Interview explanation

> “I use probe-style testing to cover specific behavior categories, record expected outcomes, and compare observed responses with those outcomes. I keep probes controlled and repeatable, and investigate unexpected results before calling them findings. This notebook is a fixture-based demonstration, not a garak scan.”

## Safe-use note

Use garak only against models and environments you are authorized to test. Prefer synthetic test data and review current garak documentation for actual probe configuration.
