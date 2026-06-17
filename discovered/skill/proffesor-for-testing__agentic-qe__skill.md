---
name: proffesor-for-testing__agentic-qe__skill
source: https://github.com/proffesor-for-testing/agentic-qe/blob/0ea5c2a684e9239748355f2ae65d1f98375ac9e9/assets/skills/observability-testing-patterns/SKILL.md
repo: proffesor-for-testing/agentic-qe
kind: skill
stars: 388
last_pushed: 2026-06-15T08:31:28Z
license: mit
score: 9
domains: [qa-engineering, devops, observability]
tags: [monitoring, dashboards, alerting, elasticsearch, grafana]
curated: 2026-06-16
curated_by: config-scout
---

# proffesor-for-testing/agentic-qe — skill

**Why it's worth keeping:** Uses a high-value 'Source Truth vs. Aggregation' validation pattern that is hard to automate without specific guidance. The hierarchical testing levels (Query -> Dashboard -> Alert) provide an excellent mental model for agents.

**Summary:** Provides structured patterns for validating observability infrastructure including dashboard accuracy, alert thresholds, and log completeness. It includes practical code templates for comparing ground-truth databases against monitoring aggregations.

**Source credibility:** High; the repository shows active maintenance and strong social proof via star count.

**Recency:** 

**Source:** [proffesor-for-testing/agentic-qe/assets/skills/observability-testing-patterns/SKILL.md](https://github.com/proffesor-for-testing/agentic-qe/blob/0ea5c2a684e9239748355f2ae65d1f98375ac9e9/assets/skills/observability-testing-patterns/SKILL.md) · 388★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: observability-testing-patterns
description: "Observability and monitoring validation patterns for dashboards, alerting, log aggregation, APM traces, and SLA/SLO verification. Use when testing monitoring infrastructure, dashboard accuracy, alert rules, or metric pipelines."
category: specialized-testing
priority: high
tokenEstimate: 1600
agents: [qe-integration-tester, qe-performance-tester, qe-visual-tester]
implementation_status: optimized
optimization_version: 1.0
last_optimized: 2026-02-04
dependencies: [api-testing-patterns, shift-right-testing]
quick_reference_card: true
tags: [observability, monitoring, kibana, elasticsearch, dashboards, alerting, metrics, logging]
trust_tier: 3
validation:
  schema_path: schemas/output.json
  validator_path: scripts/validate-config.json
  eval_path: evals/observability-testing-patterns.yaml
---

# Observability Testing Patterns

## Browser engine

Dashboard screenshot validation and alert-UI verification go through the **qe-browser** fleet skill (`.claude/skills/qe-browser/`). Vibium is installed by `aqe init`. Typical dashboard regression workflow:

```bash
vibium go "$GRAFANA_URL/d/api-latency"
vibium wait load
node .claude/skill
```

</details>
