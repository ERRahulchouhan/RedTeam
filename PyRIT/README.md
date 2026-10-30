# LLM Red-Team Tools: Experiments and Interview Guide

This folder contains one starter experiment notebook for each tool in the tool list. Each notebook has 10 safe, deterministic examples covering common AI evaluation checks.

## What is in each tool folder?

Each folder contains `experiment.ipynb`. The notebooks now use **different methods for each tool**, rather than repeating an identical test list in every folder. Every method is explained in its own Markdown cell, immediately followed by a separate Python cell that checks its example fixture. Each notebook ends with an interview summary.

Examples include PyRIT-style conversation replay and scorer calibration, garak-style probes, promptfoo-style assertions and regression checks, Giskard-style dataset and slice checks, fuzzing-style benign input variations, and benchmark-style scoring and coverage checks. These are learning examples, not integrations with the products' APIs.

The 10 test areas are:

1. **Baseline helpfulness** — does the model answer an ordinary request?
2. **Instruction boundaries** — does it preserve a simple output constraint?
3. **Synthetic-secret protection** — does it avoid echoing a fake secret?
4. **Data minimization** — does it avoid repeating synthetic contact data?
5. **Safe refusal** — does it decline a disallowed category without giving harmful details?
6. **Groundedness** — does it stick to a supplied fictional fact?
7. **Output schema** — is the response valid JSON with the expected types?
8. **Benign robustness** — do ordinary paraphrases produce consistent results?
9. **Tool authorization** — does a mock agent reject an unapproved action?
10. **Multi-turn consistency** — does it retain a harmless preference?

The notebooks use only Python's standard library and fictional fixtures. They do **not** connect to a real model, execute a red-team product, or contact an external service. The included passing results validate the example checks, not the security of any model or product.

## Run a notebook cell by cell

1. Open a tool folder and open `experiment.ipynb` in VS Code or Jupyter.
2. Select a Python 3 kernel.
3. Read each method's explanation, then run the Python cell directly below it.
4. Each example cell should print its own `PASS` message.
5. To evaluate an approved local test system, replace that test cell's `observed` fixture with a safely captured response, then run the check. Use synthetic data and systems you are authorized to test.

A failed check is a prompt to investigate, not by itself proof of a vulnerability. Record the test setup, expected behavior, observed behavior, impact, and a reproducible regression check.

## Tool folders

| Folder | Interview-level description |
|---|---|
| `PyRIT` | Organize AI red-team assessment workflows and track results. |
| `garak` | Probe language models for classes of weaknesses. |
| `promptfoo` | Compare prompts/models and keep evaluations in a repeatable workflow. |
| `DeepTeam` | Structure red-team assessments for models and agents. |
| `Giskard` | Evaluate AI systems, including model and retrieval-augmented workflows. |
| `FuzzyAI` | Explore robustness with varied test inputs. |
| `Prompt Fuzzer` | Check prompt-handling behavior across controlled variations. |
| `Inspect AI` | Build structured, repeatable model evaluations. |
| `Moonshot` | Organize AI security tests and benchmarks. |
| `CyberSecEval` | Assess model security-related capabilities using benchmark-style tests. |

These are high-level descriptions, not claims that the notebooks use each product's API. Check the tool's current documentation before connecting it to an evaluation environment.

## Interview explanation

You can describe the work like this:

> “I created a repeatable evaluation plan across several AI security tools. I cover helpfulness, instruction boundaries, synthetic-data privacy, safe refusals, groundedness, structured output, robustness, tool authorization, and multi-turn consistency. I use controlled fixtures, define expected behavior before testing, capture evidence, and convert failures into regression checks. I only test systems I am authorized to assess. The notebooks are starter fixtures; I would validate each tool's integration separately before reporting product-specific results.”

### A simple way to explain one test

- **Risk:** An agent might try to use an action outside its approved scope.
- **Test:** In a mock registry, allow a read-only demo lookup and reject an unapproved demo action.
- **Expected result:** Only the approved action runs; the other is recorded as rejected.
- **Evidence:** The observed action list and the check result.
- **Next step:** If the check fails in an authorized environment, investigate the control, document impact, fix it, and add a regression test.

## Responsible-use notes

- Use a local or explicitly approved environment and follow its rules.
- Keep secrets, personal information, and real customer data out of these fixtures.
- Do not treat a passing mock test as a real security certification.
- Report findings with enough evidence to reproduce them safely, and verify fixes with regression tests.
