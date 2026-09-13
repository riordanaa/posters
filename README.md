# Aidan Riordan — posters, papers, talks

PhD student in Industrial Engineering, Northeastern University (operations research: simulation-optimization
of pharmaceutical supply chains under drug shortages). Contact: riordan.a@northeastern.edu

## Posters

### [Why Can Large Language Models Optimize?](2025-optimization-days-llm-metaheuristic-poster.pdf)
*Optimization Days 2025, Montréal · NSF NRT poster session, Northeastern — first author, presenter*

Can an LLM re-implement a published optimization algorithm from the paper alone? We gave Claude Sonnet 4 and
Gemini 2.5 Pro a research paper describing a Variable Neighborhood Search algorithm for a clustering problem
(original code never released) and asked them to produce code matching the original's performance. A
Context–Communication–Iteration prompting framework structures the exchange; the resulting implementations
reach about 90% of the published performance. The poster reports the benchmark, where the models fail, and
what that says about LLMs as research assistants for metaheuristics.

### [Evolutionary algorithm for inferring differential equations](2025-dynamics-days-evolutionary-diffeq-poster.pdf)
*Dynamics Days 2025 — with W. Garrett Mitchener (College of Charleston) — co-author*

Symbolic regression that recovers the governing equations of a physical system from sampled data. Jessamine
is a flexible evolutionary framework in which each candidate model is a linear combination of evolved
functions, fitted in three layers: ridge regression for the linear weights, a general minimizer for scalar
parameters, and an evolutionary search over the functions themselves (with variable-neighborhood-style
escapes when innovation stalls). As a test case it recovers the Brusselator reaction–diffusion PDEs exactly
from synthesized samples of the fields and their spatial derivatives. Code: [Jessamine.jl](https://github.com/wgm-applied-math/Jessamine.jl).

## Papers

| Item | Venue | Role |
|---|---|---|
| **Large Language Models for Metaheuristic Implementation: A Case Study with Variable Neighborhood Search** | Under review, *Journal of Heuristics*, 2025 | First author (preprint on request) |
| **Interpretability, Adaptability and Scalability of Variable Neighborhood Search** (with Pierre Hansen and Xavier Hansen) | 15th Metaheuristics International Conference (MIC 2024), Lorient, France — Springer LNCS | Co-author, presenter |
| **The Jessamine Symbolic Regression System and a Reliability Approach to Benchmarking** | Submitted, *Evolutionary Computation* | Co-author (manuscript on request) |

Posters are the versions presented at the venues listed.
