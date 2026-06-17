---
name: foryourhealth111-pixel__Vibe-Skills
source: https://github.com/foryourhealth111-pixel/Vibe-Skills/blob/25ab877ad0e2b0631c28399772941b9f35401b0b/SKILL.md
repo: foryourhealth111-pixel/Vibe-Skills
kind: skill
stars: 2290
last_pushed: 2026-05-19T15:42:16Z
license: apache-2.0
score: 9
domains: [agents-ai, cli-tools, orchestration]
tags: [governance, state-machine, workflow-automation]
curated: 2026-06-14
curated_by: config-scout
---

# foryourhealth111-pixel/Vibe-Skills — skill

**Why it's worth keeping:** The implementation of 'progressive governed stops' and 'bounded re-entry' via structured JSON decision files is an elite pattern for preventing agent drift in complex tasks. The protocol enforces rigorous state transitions rather than relying on loose chat history.

**Summary:** A sophisticated governance protocol that transforms an AI agent from a chat-based assistant into a structured state machine. It uses explicit stages (Requirements -> Plan -> Execution) and formal JSON 'contracts' to ensure human oversight before proceeding.

**Source credibility:** Highly regarded repository with significant stars, indicating a mature framework.

**Recency:** 

**Source:** [foryourhealth111-pixel/Vibe-Skills/SKILL.md](https://github.com/foryourhealth111-pixel/Vibe-Skills/blob/25ab877ad0e2b0631c28399772941b9f35401b0b/SKILL.md) · 2290★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: vibe
description: Vibe Code Orchestrator (VCO) is a governed runtime entry that freezes requirements, plans XL-first execution, and enforces verification and phase cleanup.
---

# Vibe Governed Runtime Entry

This file is the host-facing SOP for entering canonical `vibe`. Keep it small:
runtime details belong in `protocols/runtime.md`, execution discipline belongs in
`protocols/do.md`, and host wrapper recipes belong in installer-generated wrapper
docs.

## Trigger Contract

Enter canonical `vibe` before ordinary execution when the user explicitly invokes
`$vibe`, `/vibe`, or the `vibe` skill, or when the host intentionally chooses
governed requirement/plan/execution closure for a complex task.

Do not route every loosely related task into `vibe`. Lightweight questions,
single-command checks, or tasks better served by another explicitly requested
skill may proceed outside `vibe` unless the user explicitly invoked this entry.

`vibe-upgrade` is a separate public skill for upgrading the installed
Vibe-Skills project. Do not relaunch an upgrade request as `entry_id = vibe`;
use the `vibe-upgrade` skill and its backend instead.

User instructions remain highest priority. If C
```

</details>
