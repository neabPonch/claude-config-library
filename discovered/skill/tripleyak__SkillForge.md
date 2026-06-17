---
name: tripleyak__SkillForge
source: https://github.com/tripleyak/SkillForge/blob/92d8d87aadc88df915e88be3ceccc6ed16a920ce/SKILL.md
repo: tripleyak/SkillForge
kind: skill
stars: 694
last_pushed: 2026-05-24T15:41:21Z
license: mit
score: 9
domains: [agents-ai, automation, orchestration]
tags: [meta-skill, orchestrator, framework]
curated: 2026-06-14
curated_by: config-scout
---

# tripleyak/SkillForge — skill

**Why it's worth keeping:** The 'Synthesis Panel' pattern (requiring unanimous agent approval) and the multi-phase workflow (Triage to Generation) are excellent templates for high-reliability tool creation.

**Summary:** A sophisticated meta-skill orchestrator that manages the lifecycle of other skills through structured triage, deep analysis, and multi-agent verification.

**Source credibility:** Strong; significant star count (694) and very recent updates indicate a high-quality, community-vetted project.

**Recency:** Highly current, utilizing modern Claude models and advanced agentic orchestration techniques.

**Source:** [tripleyak/SkillForge/SKILL.md](https://github.com/tripleyak/SkillForge/blob/92d8d87aadc88df915e88be3ceccc6ed16a920ce/SKILL.md) · 694★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: skillforge
description: "Intelligent skill router, proactive advisor, and creator. Analyzes ANY input to recommend existing skills, improve them, or create new ones. Adds proactive Context Skill Advisor suggestions from session, project, and personal context using user-controlled Proactivity Levels."
license: MIT
model: claude-opus-4-5-20251101
user-invocable: true
allowed-tools:
  - Read
  - Glob
  - Grep
  - Bash
  - Write
  - Edit
metadata:
  version: 5.2.0
  subagent_model: claude-opus-4-5-20251101
  domains: [meta-skill, automation, skill-creation, orchestration, agentic, routing]
  type: orchestrator
  inputs: [any-input, user-goal, domain-hints]
  outputs: [SKILL.md, references/, scripts/, SKILL_SPEC.md, recommendations]
---

# SkillForge 5.2 - Intelligent Skill Router, Advisor & Creator

Analyzes ANY input to find, improve, or create the right skill. It can also proactively surface evidence-backed skill suggestions through the Context Skill Advisor.

---

## Quick Start

**Any input works.** SkillForge will intelligently route to the right action:

```
# These all work - SkillForge figures out what you need:

SkillForge: create a skill for automated code review
→
```

</details>
