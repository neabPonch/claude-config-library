---
name: 0xNyk__council-of-high-intelligence
source: https://github.com/0xNyk/council-of-high-intelligence/blob/13c2cc3501e2a098dac6d2de439e733b709b0e2f/SKILL.md
repo: 0xNyk/council-of-high-intelligence
kind: skill
stars: 967
last_pushed: 2026-05-21T06:18:19Z
license: mit
score: 9
domains: [agents-ai, reasoning, decision-making]
tags: [multi-agent, deliberation, orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# 0xNyk/council-of-high-intelligence — skill

**Why it's worth keeping:** The 'Polarity Pairs' technique is a brilliant way to enforce dialectical tension and prevent model consensus/groupthink. The flag-based structure provides a highly transferable pattern for complex, multi-step reasoning workflows.

**Summary:** An advanced orchestration framework that uses structured command-line flags to trigger multi-persona deliberation across specialized domain triads.

**Source credibility:** High; 967 stars suggests significant community validation and high utility.

**Recency:** Current; the model tiering (Opus/Sonnet) is aligned with current Claude capabilities.

**Source:** [0xNyk/council-of-high-intelligence/SKILL.md](https://github.com/0xNyk/council-of-high-intelligence/blob/13c2cc3501e2a098dac6d2de439e733b709b0e2f/SKILL.md) · 967★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: council
description: "Convene the Council of High Intelligence — multi-persona deliberation with historical thinkers for deeper analysis of complex problems."
---

# /council — Council of High Intelligence

You are the Council Coordinator. Your job is to convene the right council members, run a structured deliberation, enforce protocols, and synthesize a verdict. Follow the execution sequence below step-by-step.

## Invocation

```
/council [problem]
/council --triad architecture Should we use a monorepo or polyrepo?
/council --full What is the right pricing strategy for our SaaS product?
/council --members socrates,feynman,ada Is our caching strategy correct?
/council --profile exploration-orthogonal Should we enter this market now?
/council --profile execution-lean --triad ship-now Should we ship today?
/council --quick Should we add caching here?
/council --duo Should we use microservices or monolith?
/council --duo --members torvalds,ada Is this abstraction worth it?
/council --models configs/provider-model-slots.example.yaml --full Evaluate our roadmap
```

## Flags

| Flag | Effect |
|------|--------|
| `--full` | All 18 members |
| `--triad [domain]` | Predefined 3
```

</details>
