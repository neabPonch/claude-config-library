---
name: andylizf__nonstop
source: https://github.com/andylizf/nonstop/blob/9511b6f94b38482b54952e18f0df2dae2b97961a/SKILL.md
repo: andylizf/nonstop
kind: skill
stars: 262
last_pushed: 2026-04-04T01:16:03Z
license: mit
score: 9
domains: [agents-ai, cli-tools, devops]
tags: [autonomous, afk-mode, risk-management]
curated: 2026-06-14
curated_by: config-scout
---

# andylizf/nonstop — skill

**Why it's worth keeping:** The 'Dangerous Operations Manifest' for granular permissioning and the three-level blocker decision framework are top-tier patterns for reliable agent autonomy.

**Summary:** Provides a sophisticated 'AFK' mode that enables continuous autonomous work through pre-flight risk assessment and explicit permission manifests.

**Source credibility:** High; 262 stars indicates a well-vetted tool used by many in the community.

**Recency:** Current; updated within the last two months to align with modern workflows.

**Source:** [andylizf/nonstop/SKILL.md](https://github.com/andylizf/nonstop/blob/9511b6f94b38482b54952e18f0df2dae2b97961a/SKILL.md) · 262★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nonstop
description: Autonomous work mode that lets Claude work continuously while the user is away. Activates pre-flight risk assessment, dangerous-ops approval, and a blocker decision framework. Use "/nonstop" to activate, "/nonstop off" to deactivate. Use this skill whenever the user says things like "go nonstop", "keep working", "don't stop", "I'm going AFK", "work while I sleep", "finish this without me", or wants Claude to work autonomously without interruption.
---

# Nonstop Mode

A session-scoped autonomous work mode. When activated, Claude works continuously without stopping to ask the user, handling blockers intelligently.

## Activation — `/nonstop` or `/nonstop on`

When the user triggers nonstop mode, **start the pre-flight sequence immediately**. Drop whatever else you are doing — do not wait for background agents, pending reads, or other in-progress work. The pre-flight is the priority now.

Complete the pre-flight **before doing any work**. The pre-flight exists because once the user walks away, there is no one to answer questions — every ambiguity must be resolved now.

### Phase 1: Mental Simulation — Anticipate Every Blocker

Mentally simulate the enti
```

</details>
