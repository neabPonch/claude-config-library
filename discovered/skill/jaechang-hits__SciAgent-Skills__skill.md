---
name: jaechang-hits__SciAgent-Skills__skill
source: https://github.com/jaechang-hits/SciAgent-Skills/blob/02745ef6988d5949cd2bd8091307c14047faa833/skills/scientific-computing/pymoo/SKILL.md
repo: jaechang-hits/SciAgent-Skills
kind: skill
stars: 200
last_pushed: 2026-06-15T09:53:48Z
license: other
score: 9
domains: [data-science, optimization, mathematics, python]
tags: [evolutionary-algorithms, multi-objective, optimization]
curated: 2026-06-15
curated_by: config-scout
---

# jaechang-hits/SciAgent-Skills — skill

**Why it's worth keeping:** Uses a modular structure that allows agents to jump between specific API sections; includes crucial high-level nuances like vectorization benefits and hyperparameter 'eta' contexts.

**Summary:** A highly structured technical reference for the pymoo optimization framework, covering problem definition, algorithm selection, and operator tuning.

**Source credibility:** High; part of a specialized bioinformatics repository (SciAgent) with significant community traction.

**Recency:** Current; follows modern Pythonic implementation patterns suitable for contemporary AI coding tasks.

**Source:** [jaechang-hits/SciAgent-Skills/skills/scientific-computing/pymoo/SKILL.md](https://github.com/jaechang-hits/SciAgent-Skills/blob/02745ef6988d5949cd2bd8091307c14047faa833/skills/scientific-computing/pymoo/SKILL.md) · 200★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "pymoo"
description: "Python framework for single- and multi-objective optimization with evolutionary algorithms. Define vectorized objectives and constraints; solve with NSGA-II, NSGA-III, MOEA/D, GAs, or differential evolution. Analyze Pareto fronts, visualize trade-offs, customize operators and callbacks. For engineering design, hyperparameter search, and conflicting objectives. Alternatives: scipy.optimize (single-objective, gradient), platypus, jMetalPy (Java)."
license: "Apache-2.0"
---

# pymoo

## Overview

pymoo provides a unified API for multi-objective optimization via population-based evolutionary algorithms. Users define a problem by subclassing `Problem` or `ElementwiseProblem`, specifying objectives (`n_obj`), decision variables (`n_var`), and optional constraints (`n_ieq_constr`). Algorithms like NSGA-II and NSGA-III return a `Result` object containing the Pareto-optimal population, objective values, and decision variable values. pymoo separates problem definition, algorithm configuration, operator selection, and analysis — each component is independently replaceable.

## When to Use

- Optimizing a design with two or more conflicting objectives (e.g., min
```

</details>
