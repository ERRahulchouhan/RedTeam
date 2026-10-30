# Moonshot Experiment Guide

## What this folder is for

This folder contains a cell-by-cell notebook of safe, fictional benchmark and scorecard examples. It does **not** execute Moonshot, run a benchmark product, or contact a model.

## Methods in `experiment.ipynb`

1. Benchmark case execution
2. Benchmark suite coverage
3. Scorecard threshold
4. Repeat-run stability
5. Reference comparison
6. Output schema case
7. Risk-label matrix
8. Regression scorecard
9. Action boundary case
10. Aggregate pass-rate report

Read the explanation for each benchmark method, then run its check cell. The fixtures are examples for teaching reproducible evaluation, not product results.

## Interview explanation

> “I design benchmark cases with clear labels, coverage goals, score thresholds, and regression comparisons. I report aggregate metrics together with the underlying test scope and limitations. This notebook is a local scorecard demonstration, not a Moonshot benchmark run.”

## Safe-use note

Use only authorized targets and approved datasets. Consult current Moonshot documentation before connecting an evaluation to a real model or service.
