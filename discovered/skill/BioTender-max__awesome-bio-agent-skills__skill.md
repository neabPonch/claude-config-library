---
name: BioTender-max__awesome-bio-agent-skills__skill
source: https://github.com/BioTender-max/awesome-bio-agent-skills/blob/2aea21b3e2973d15eca5e372153ae092860d4a7c/skills/sciagent/pymoo/SKILL.md
repo: BioTender-max/awesome-bio-agent-skills
kind: skill
stars: 58
last_pushed: 2026-06-14T15:36:47Z
license: other
score: 9
domains: [data-science, mathematical-optimization, python]
tags: [optimization, evolutionary-algorithms, pymoo]
curated: 2026-06-15
curated_by: config-scout
---

# BioTender-max/awesome-bio-agent-skills — skill

**Why it's worth keeping:** It breaks down complex workflows into modular components (Problem, Algorithm, Operator, Termination), allowing an agent to compose custom evolutionary algorithms rather than just following a single template.

**Summary:** A highly structured technical guide for the `pymoo` optimization framework, covering everything from problem definition to termination criteria.

**Source credibility:** High; sourced from a specialized biomedical research repository with recent maintenance.

**Recency:** Current; follows modern Python idioms and provides specific hyperparameter tuning guidance relevant to contemporary AI coding tasks.

**Source:** [BioTender-max/awesome-bio-agent-skills/skills/sciagent/pymoo/SKILL.md](https://github.com/BioTender-max/awesome-bio-agent-skills/blob/2aea21b3e2973d15eca5e372153ae092860d4a7c/skills/sciagent/pymoo/SKILL.md) · 58★

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
