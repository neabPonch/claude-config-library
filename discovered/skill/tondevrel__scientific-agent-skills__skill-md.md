---
name: tondevrel__scientific-agent-skills__skill-md
source: https://github.com/tondevrel/scientific-agent-skills/blob/6e89d9e8c84188050bd50c420e48b639be484bb9/skills/dowhy/SKILL.MD
repo: tondevrel/scientific-agent-skills
kind: skill
stars: 15
last_pushed: 2026-02-01T04:41:56Z
license: mit
score: 9
domains: [data-science, statistical-analysis]
tags: [python, dowhy, causal-inference, statistics]
curated: 2026-06-15
curated_by: config-scout
---

# tondevrel/scientific-agent-skills — skill

**Why it's worth keeping:** It includes high-level reasoning guides like 'Critical Rules' and 'Anti-Patterns' that teach an agent how to avoid statistical fallacies rather than just providing syntax.

**Summary:** Provides a structured mental model and workflow—Identify, Estimate, Refute—for performing causal inference using the DoWhy library.

**Source credibility:** Specific scientific toolset; 15 stars indicates a niche but respected domain interest.

**Recency:** Very recent (last pushed 4 months ago), making it highly relevant for modern workflows.

**Source:** [tondevrel/scientific-agent-skills/skills/dowhy/SKILL.MD](https://github.com/tondevrel/scientific-agent-skills/blob/6e89d9e8c84188050bd50c420e48b639be484bb9/skills/dowhy/SKILL.MD) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: dowhy
description: Causal inference framework for answering "does X cause Y?" beyond correlation. DoWhy (Microsoft Research) provides the identify-estimate-refute loop: define a causal graph (DAG), identify the causal effect using backdoor/frontdoor/instrumental variable criteria, estimate treatment effects with multiple estimators, and validate results with automated refutation tests. Use when: distinguishing causation from correlation, estimating treatment effects (ATE, ATT, CATE), designing and analyzing A/B tests with confounders, using instrumental variables, performing counterfactual reasoning ("what would have happened if..."), validating causal claims with sensitivity analysis, working with observational data where randomization is impossible, or any analysis where the question is "what is the CAUSAL effect of X on Y" rather than just "how do X and Y relate?"
version: 0.11.0
license: MIT
---

# DoWhy — Causal Inference

DoWhy answers the question every analyst actually wants answered: **"Does X cause Y, or is it just correlated?"** Correlation is everywhere. Causation requires structure — a causal graph that encodes which variables influence which. DoWhy's workflo
```

</details>
