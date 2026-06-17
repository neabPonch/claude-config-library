---
name: MHaggis__Security-Detections-MCP__skill
source: https://github.com/MHaggis/Security-Detections-MCP/blob/4cd04c80d1c744734ea6288cb6b7405aa18ed174/.claude/skills/spl-optimizer/SKILL.md
repo: MHaggis/Security-Detections-MCP
kind: skill
stars: 444
last_pushed: 2026-04-21T00:04:08Z
license: unknown
score: 9
domains: [security, data-engineering]
tags: [siem, splunk, kql, optimization, detection-engineering]
curated: 2026-06-16
curated_by: config-scout
---

# MHaggis/Security-Detections-MCP — skill

**Why it's worth keeping:** Uses highly effective 'Bad vs. Good' code comparisons and includes a command cost reference that allows an agent to reason about performance trade-offs.

**Summary:** Provides expert-level optimization patterns for SIEM query languages including Splunk (SPL), Microsoft Sentinel (KQL), and Elastic (EQL/ES|QL).

**Source credibility:** High; the source repository has significant community interest (444 stars) and specialized security focus.

**Recency:** Current; focuses on modern SIEM optimization techniques used in production environments today.

**Source:** [MHaggis/Security-Detections-MCP/.claude/skills/spl-optimizer/SKILL.md](https://github.com/MHaggis/Security-Detections-MCP/blob/4cd04c80d1c744734ea6288cb6b7405aa18ed174/.claude/skills/spl-optimizer/SKILL.md) · 444★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: Detection Query Optimizer
description: Optimize detection queries for performance across Splunk (SPL), Microsoft Sentinel (KQL), and Elastic Security (EQL/ES|QL). Covers search pipeline internals, common anti-patterns, and optimization techniques for detection rules on each platform.
---

# Detection Query Optimizer Skill

## Overview

Every SIEM processes queries differently. Understanding the execution model is essential for writing detections that run fast enough for scheduled execution without excessive resource consumption. This skill covers optimization for the three major query languages.

**Set `$SIEM_PLATFORM`** to focus guidance: `splunk`, `sentinel`, `elastic`

## Quick Reference: Which Section?

| Platform | Query Language | Section |
|----------|---------------|---------|
| Splunk Enterprise / Cloud | SPL | [SPL Optimization](#spl-optimization-splunk) |
| Microsoft Sentinel / Defender | KQL | [KQL Optimization](#kql-optimization-microsoft-sentinel) |
| Elastic Security | EQL / ES\|QL | [EQL/ES\|QL Optimization](#eqlesql-optimization-elastic-security) |
| Sigma | N/A | Optimization happens at the backend/compiler level. Write clean Sigma; let pySigma optimize
```

</details>
