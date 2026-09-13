# Aidan Riordan — posters, papers, talks

PhD student in Industrial Engineering, Northeastern University (operations research: simulation-optimization
of pharmaceutical supply chains under drug shortages). Contact: riordan.a@northeastern.edu

## Papers

### [Large Language Models for Metaheuristic Implementation: A Case Study with Variable Neighborhood Search](https://link.springer.com/chapter/10.1007/978-3-032-19582-1_11)
*Springer Lecture Notes in Computer Science, 2025 — first author*

Metaheuristics are widely used in combinatorial optimization but take real expertise and engineering effort
to implement. We ask whether current LLMs can turn a state-of-the-art algorithm description into performant
code with minimal human intervention. We introduce a generalizable prompting framework — Context,
Communication, Iteration (CCI) — and use it to replicate a Variable Neighborhood Search for the balanced
minimum sum-of-squares clustering problem with Gemini 2.5 Pro and Claude Sonnet 4. Gemini's implementation
came within 0.032% of the reference on average (median 0.009%), statistically non-inferior within a 0.01%
margin, and it corrected a missing term in the neighborhood-evaluation formula as printed in the source
paper; Claude did not. LLM-assisted engineering looks like a viable path to making high-performance
methods accessible to more researchers. An extended version is under review at the *Journal of Heuristics*.

### [Interpretability, Adaptability and Scalability of Variable Neighborhood Search](https://link.springer.com/chapter/10.1007/978-3-031-62912-9_30)
*Springer Lecture Notes in Computer Science, June 2024 — 15th Metaheuristics International Conference (MIC 2024), Lorient, France — co-author with Pierre Hansen and Xavier Hansen; presenter*

Twenty-five years on, Variable Neighborhood Search remains an effective and accessible metaheuristic. The
paper argues that its way of escaping local optima gives it three properties that suit large, complex
real-world problems: interpretability (a simple modular design that invites problem analysis and systematic
formulation of the search space), adaptability (it hybridizes naturally with other methods) and scalability
(it parallelizes and integrates AI/ML components readily). It closes with recommendations for the community:
public code repositories and problem libraries, documented real-world implementations, engagement across
metaheuristics, and popularizing VNS as an accessible technique.

### The Jessamine Symbolic Regression System and a Reliability Approach to Benchmarking
*Submitted, Evolutionary Computation — co-author (manuscript on request)*

## Posters

### [Why Can Large Language Models Optimize?](2025-optimization-days-llm-metaheuristic-poster.pdf)
*Optimization Days 2025, Montréal · NSF NRT poster session, Northeastern — first author, presenter*

The poster version of the LLM-replication study above: give the model only the paper describing a VNS
algorithm (the original code was never released) and ask for code that matches the original's performance.
It shows the CCI prompting framework, the benchmark against the reference implementation, where the models
fail, and what that says about LLMs as research assistants for metaheuristics.

### [Evolutionary algorithm for inferring differential equations](2025-dynamics-days-evolutionary-diffeq-poster.pdf)
*Dynamics Days 2025 — with W. Garrett Mitchener (College of Charleston) — co-author*

Symbolic regression that recovers the governing equations of a physical system from sampled data. Jessamine
is a flexible evolutionary framework in which each candidate model is a linear combination of evolved
functions, fitted in three layers: ridge regression for the linear weights, a general minimizer for scalar
parameters, and an evolutionary search over the functions themselves (with variable-neighborhood-style
escapes when innovation stalls). As a test case it recovers the Brusselator reaction–diffusion PDEs exactly
from synthesized samples of the fields and their spatial derivatives. Code: [Jessamine.jl](https://github.com/wgm-applied-math/Jessamine.jl).

### [An Interpretable Machine Learning Method in Symbolic Regression — Jessamine](2024-surf-interpretable-ml-jessamine-poster.pdf)
*College of Charleston SURF (Summer Undergraduate Research) grant, 2024 — advisor W. Garrett Mitchener — author, presenter*

Black-box models are used for high-stakes decisions in healthcare and criminal justice, where a prediction
without a readable reason is a liability. This project asks whether an interpretable model can keep up.
Jessamine is a genetic-algorithm symbolic-regression system: each genome is a candidate function, populations
are mutated and recombined, the best are simplified into short algebraic expressions. Two results on the
poster: Jessamine's evolved features let XGBoost capture non-linear structure with a far simpler ensemble
than it needs on raw inputs, and on a 303-patient heart-disease dataset it surfaces the three predictors a
cardiologist would expect (ST depression, maximum heart rate, exercise-induced angina) while stating
honestly where its accuracy still trails black-box models.

Posters are the versions presented at the venues listed.
