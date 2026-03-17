# Adaptive Two-Stage Stochastic Routing

Vehicle routing under **travel-time uncertainty** using a **two-stage stochastic optimization** framework: plan a nominal route in stage one, then adapt in stage two once uncertainty is realized.

---

## Overview

The goal is to minimize **expected total cost** (operating cost + penalties for time-window violations) by combining:

- **Stage 1** — Deterministic routing under nominal travel times
- **Stage 2** — Scenario-dependent recourse with time-indexed traversal, waiting decisions, and early/late service penalties (constant, linear, or quadratic)

The model is formulated as a **Mixed-Integer Linear Program (MILP)** with finite travel-time scenarios and known probabilities.

---

## Key results

Adaptive recourse consistently improves performance over non-adaptive execution:

| Penalty type | Improvement |
|--------------|-------------|
| Constant     | ~20%        |
| Linear       | ~20%        |
| Quadratic    | ~20%        |

The benefit of adaptivity holds across different operating-cost levels.

---

## Repo structure

- **`Code/`** — Implementation and notebooks
- **`Data/`** — Input data and scenarios
- **`report.pdf`** — Full write-up and analysis

---

## Keywords

Stochastic programming · Vehicle routing · MILP · Two-stage optimization · Time windows
