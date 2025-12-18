# Model Card: Black-Box Bayesian Optimisation Strategy

## Overview
**Model name:** BBO Capstone Optimisation Strategy  
**Type:** Iterative black-box optimisation using surrogate models  
**Version:** v1.0 (Weeks 1–10)

This model represents an iterative optimisation strategy designed to explore and exploit unknown objective functions using limited query budgets.

---

## Intended Use
**Primary use:**
- Optimising unknown black-box functions with limited evaluations
- Educational experimentation with Bayesian optimisation strategies

**Out-of-scope use:**
- Real-time or safety-critical optimisation
- High-stakes decision-making without uncertainty guarantees

---

## Optimisation Strategy Details
The approach evolved across ten rounds of optimisation:
- Early rounds focused on broad exploration using random and space-filling queries
- Mid rounds introduced surrogate modelling (e.g. Gaussian Processes, regression-based approximations)
- Later rounds prioritised local exploitation around promising regions while maintaining uncertainty awareness

Acquisition decisions balanced predicted performance and uncertainty to reduce overfitting and premature convergence.

---

## Performance Summary
- Optimisation was evaluated across eight unknown functions with dimensionalities from 2D to 8D
- Performance improvements were incremental, with diminishing returns observed after later rounds
- Stability and consistency improved as the data set grew

Metrics used:
- Relative improvement over previous queries
- Consistency of high-performing regions across iterations

---

## Assumptions and Limitations
**Key assumptions:**
- Objective functions are smooth or locally continuous
- Nearby inputs produce correlated outputs

**Limitations:**
- Limited data increases uncertainty in higher-dimensional spaces
- Surrogate models may misrepresent sharp discontinuities
- Exploration is constrained by query budget

---

## Ethical and Transparency Considerations
- All optimisation decisions are documented and reproducible
- Assumptions, limitations and failure modes are explicitly stated
- Transparency supports auditability and responsible reuse of the approach

This model card aims to support interpretability, reproducibility and responsible experimentation in black-box optimisation.
