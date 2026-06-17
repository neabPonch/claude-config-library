---
name: math-inc__OpenGauss__skill
source: https://github.com/math-inc/OpenGauss/blob/f87633900ae185b8037bf451a914fe7eeae1eb08/optional-skills/security/oss-forensics/SKILL.md
repo: math-inc/OpenGauss
kind: skill
stars: 1223
last_pushed: 2026-04-05T16:41:18Z
license: mit
score: 9
domains: [security, forensics, agents-ai, devops]
tags: [supply-chain, git-forensics, multi-agent, incident-response]
curated: 2026-06-15
curated_by: config-scout
---

# math-inc/OpenGauss — skill

**Why it's worth keeping:** The 'Role Boundary' pattern (preventing source contamination) and the mandatory evidence-citation system (EV-XXXX) are elite patterns for high-stakes agentic tasks.

**Summary:** A professional-grade forensic investigation framework that uses specialized sub-agents with strict role boundaries and rigorous anti-hallucination guardrails.

**Source credibility:** High; the repository is active and the skill exhibits a level of technical depth far beyond generic AI prompts.

**Recency:** Very current; it leverages advanced multi-agent orchestration concepts highly relevant to modern Claude Code workflows.

**Source:** [math-inc/OpenGauss/optional-skills/security/oss-forensics/SKILL.md](https://github.com/math-inc/OpenGauss/blob/f87633900ae185b8037bf451a914fe7eeae1eb08/optional-skills/security/oss-forensics/SKILL.md) · 1223★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: oss-forensics
description: |
  Supply chain investigation, evidence recovery, and forensic analysis for GitHub repositories.
  Covers deleted commit recovery, force-push detection, IOC extraction, multi-source evidence
  collection, hypothesis formation/validation, and structured forensic reporting.
  Inspired by RAPTOR's 1800+ line OSS Forensics system.
category: security
triggers:
  - "investigate this repository"
  - "investigate [owner/repo]"
  - "check for supply chain compromise"
  - "recover deleted commits"
  - "forensic analysis of [owner/repo]"
  - "was this repo compromised"
  - "supply chain attack"
  - "suspicious commit"
  - "force push detected"
  - "IOC extraction"
toolsets:
  - terminal
  - web
  - file
  - delegation
---

# OSS Security Forensics Skill

A 7-phase multi-agent investigation framework for researching open-source supply chain attacks.
Adapted from RAPTOR's forensics system. Covers GitHub Archive, Wayback Machine, GitHub API,
local git analysis, IOC extraction, evidence-backed hypothesis formation and validation,
and final forensic report generation.

---

## ⚠️ Anti-Hallucination Guardrails

Read these before every investigation step. Violat
```

</details>
