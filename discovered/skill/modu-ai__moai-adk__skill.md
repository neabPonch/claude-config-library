---
name: modu-ai__moai-adk__skill
source: https://github.com/modu-ai/moai-adk/blob/8a9c1062fe4f89fee16270a392e62a44ca4eaf98/internal/template/templates/.claude/skills/moai-ref-testing-pyramid/skill.md
repo: modu-ai/moai-adk
kind: skill
stars: 1074
last_pushed: 2026-06-15T04:40:14Z
license: apache-2.0
score: 9
domains: [software-engineering, testing, quality-assurance]
tags: [tdd, test-pyramid, qa-standards, agentic-instructions]
curated: 2026-06-15
curated_by: config-scout
---

# modu-ai/moai-adk — skill

**Why it's worth keeping:** It includes an actionable 'Verification' checklist and 'Red Flags' section that allow an agent to self-audit its work against high-quality standards.

**Summary:** A comprehensive testing standard providing quantitative pyramid ratios, coverage targets, and specific code patterns to guide agentic development.

**Source credibility:** Highly credible; part of a well-maintained, high-star spec-first agentic development kit.

**Recency:** Very current, utilizing advanced agentic metadata and progressive disclosure techniques.

**Source:** [modu-ai/moai-adk/internal/template/templates/.claude/skills/moai-ref-testing-pyramid/skill.md](https://github.com/modu-ai/moai-adk/blob/8a9c1062fe4f89fee16270a392e62a44ca4eaf98/internal/template/templates/.claude/skills/moai-ref-testing-pyramid/skill.md) · 1074★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: moai-ref-testing-pyramid
description: >
  Test pyramid strategy, coverage targets, test patterns, and quality metrics
  reference. Agent-extending skill that amplifies manager-develop and manager-quality
  expertise with production-grade testing patterns.
  NOT for: production code implementation, architecture design, DevOps, security audits.
user-invocable: false
metadata:
  version: "1.0.0"
  category: "domain"
  status: "active"
  updated: "2026-03-30"
  tags: "testing, pyramid, coverage, tdd, patterns, reference"
  agent: "manager-develop"

# MoAI Extension: Progressive Disclosure
progressive_disclosure:
  enabled: true
  level1_tokens: 100
  level2_tokens: 3000

# MoAI Extension: Triggers
triggers:
  keywords: ["test", "coverage", "tdd", "unit test", "integration", "e2e"]
  agents: ["manager-develop", "manager-quality"]
  phases: ["run"]
---

# Testing Pyramid Reference

## Target Agents

- `manager-develop` - Primary: applies patterns during test creation and coverage analysis
- `manager-develop` - Secondary: applies during RED-GREEN-REFACTOR cycles

## Test Pyramid Ratios

```
       /  E2E  \        10% — Critical user journeys only
      /----------\
     / Integ
```

</details>
