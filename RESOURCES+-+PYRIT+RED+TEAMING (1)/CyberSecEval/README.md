# CyberSecEval Experiment Guide

## What this folder is for

This folder contains a cell-by-cell notebook with fictional, defensive evaluation examples. It focuses on high-level classification, safe refusals, synthetic canaries, grounding, and benchmark metrics. It does **not** run CyberSecEval or assess a live model.

## Methods in `experiment.ipynb`

1. Security knowledge classification
2. Safe refusal evaluation
3. Sensitive-data canary evaluation
4. Benign robustness evaluation
5. Grounded benchmark answer
6. Structured benchmark result
7. Defensive task dataset
8. Mock authorization boundary
9. Regression benchmark
10. Aggregate evaluation threshold

Each method explains its objective and expected outcome. Run its Python cell to check the fictional fixture; passing is not a certification or a statement about a real model.

## Interview explanation

> “I evaluate security-related model behavior with safe, defensive task categories, explicit expected outcomes, and repeatable benchmark checks. I report the scope and limitations rather than treating one score as proof of security. This notebook illustrates the approach using synthetic fixtures only.”

## Safe-use note

Keep evaluations defensive, authorized, and synthetic where possible. Follow current CyberSecEval documentation and the rules of the environment being assessed.
