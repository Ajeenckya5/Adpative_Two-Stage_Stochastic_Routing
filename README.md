# Adaptive Two-Stage Stochastic Routing

---

## Overview
This project studies **adaptive vehicle routing under travel-time uncertainty** using a **two-stage stochastic optimization framework**. A nominal route is planned in the first stage using baseline travel times, while the second stage adapts execution after uncertainty is realized through time-indexed traversal and waiting decisions.

The goal is to minimize **expected total cost**, combining operating cost and penalties for time-window violations.

---

## Model Summary
- **Stage 1:** Deterministic routing under nominal travel times  
- **Stage 2:** Scenario-dependent recourse with:
  - Time-indexed traversal
  - Waiting decisions
  - Early/late service penalties (constant, linear, quadratic)
- **Formulation:** Mixed-Integer Linear Program (MILP)
- **Uncertainty:** Finite travel-time scenarios with known probabilities

---

## Key Results
Adaptive recourse consistently improves performance compared to non-adaptive execution.

| Penalty Type | Improvement |
|-------------|------------|
| Constant    | ~20%       |
| Linear      | ~20%       |
| Quadratic   | ~20%       |

The benefit of adaptivity remains robust across different operating-cost levels.
