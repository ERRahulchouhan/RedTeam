# Inspect AI Experiment Guide

## What this folder is for

This folder contains a cell-by-cell notebook demonstrating structured evaluation concepts: task samples, response assertions, scoring, transcript checks, and aggregate metrics. It does **not** execute Inspect AI or call a model.

## Methods in `experiment.ipynb`

1. Task dataset sample
2. Solver response assertion
3. Scorer threshold
4. Conversation transcript check
5. Refusal scorer
6. JSON scorer
7. Reference-answer comparison
8. Sample consistency check
9. Tool-use transcript check
10. Evaluation pass-rate metric

Each method has an explanation cell followed by a runnable check against a fictional local fixture. A passing sample does not establish a real evaluation score.

## Interview explanation

> “I make evaluations structured around task samples, explicit solvers and scorers, and measurable aggregate results. I inspect transcript evidence and define thresholds before reviewing outcomes. This notebook teaches the structure but is not an Inspect AI evaluation run.”

## Safe-use note

For actual evaluations, follow current Inspect AI documentation, use an authorized model and task dataset, and document sampling and scoring limitations.
