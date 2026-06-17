---
name: pymc-labs__python-analytics-skills__skill
source: https://github.com/pymc-labs/python-analytics-skills/blob/5d0b7816be3b50dbf0e1e1dc14119089376b5c29/skills/pymc-testing/SKILL.md
repo: pymc-labs/python-analytics-skills
kind: skill
stars: 50
last_pushed: 2026-05-25T10:45:16Z
license: unknown
score: 8
domains: [data-science, bayesian-modeling, testing]
tags: [pymc, pytest, mcmc, unit-testing]
curated: 2026-06-15
curated_by: config-scout
---

# pymc-labs/python-analytics-skills — skill

**Why it's worth keeping:** Distinguishes between speed/use-case trade-offs of mock vs real sampling and provides concrete patterns for mocking complex sample_stats structures.

**Summary:** Provides specialized instructions for testing PyMC models by mocking expensive MCMC sampling with fast prior predictive sampling.

**Source credibility:** Highly credible; maintained by PyMC Labs, the core developers of the PyMC library.

**Recency:** Current; uses modern PyMC testing utilities and pytest fixture patterns.

**Source:** [pymc-labs/python-analytics-skills/skills/pymc-testing/SKILL.md](https://github.com/pymc-labs/python-analytics-skills/blob/5d0b7816be3b50dbf0e1e1dc14119089376b5c29/skills/pymc-testing/SKILL.md) · 50★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pymc-testing
description: >
  Testing PyMC models with pytest. Use when writing unit tests for Bayesian models,
  setting up test fixtures, mocking MCMC sampling, or testing model structure.
  Covers pymc.testing.mock_sample, pytest fixtures, and the distinction between
  fast structure-only tests (mocking) and slow posterior inference tests.
  Triggers on: testing PyMC, pytest, unit tests for models, mock sampling,
  test fixtures, CI/CD for Bayesian models.
---

# PyMC Testing

PyMC provides testing utilities to speed up test suites by mocking MCMC sampling with prior predictive sampling. This is useful for checking model structure without running expensive inference.

## Mock Sampling vs Real Sampling

| Aspect | Mock Sampling | Real Sampling |
|--------|---------------|---------------|
| Speed | Fast (seconds) | Slow (minutes) |
| Use case | Model structure, downstream code | Posterior values, convergence |
| Output | `prior`, `prior_predictive` | Full `posterior`, `sample_stats`, warmup groups |
| Divergences | Mocked (configurable) | Real diagnostics |

**Use mocking when**: Testing model specification, CI/CD pipelines, plotting code, API integration, serialization.
```

</details>
