---
name: codexstar69__bug-hunter__skill
source: https://github.com/codexstar69/bug-hunter/blob/8dedbbb10e93a3465e4549778587a4c40d0e673f/skills/recon/SKILL.md
repo: codexstar69/bug-hunter
kind: skill
stars: 421
last_pushed: 2026-05-01T12:18:26Z
license: mit
score: 9
domains: [security, codebase-analysis, agents-ai]
tags: [reconnaissance, threat-modeling, vulnerability-hunting]
curated: 2026-06-15
curated_by: config-scout
---

# codexstar69/bug-hunter — skill

**Why it's worth keeping:** The 'scaling strategy' which switches from file-level to domain-level classification for large codebases is a brilliant way to manage context limits. It also includes robust tool fallback logic for diverse environments.

**Summary:** A sophisticated reconnaissance skill that maps codebase architecture and identifies high-risk areas like trust boundaries and state transitions.

**Source credibility:** High; 421 stars and specialized, multi-agent focus indicate a serious security tooling project.

**Recency:** Very current; last pushed 2 months ago and utilizes modern agentic workflows.

**Source:** [codexstar69/bug-hunter/skills/recon/SKILL.md](https://github.com/codexstar69/bug-hunter/blob/8dedbbb10e93a3465e4549778587a4c40d0e673f/skills/recon/SKILL.md) · 421★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: recon
description: "Codebase reconnaissance agent for Bug Hunter. Maps architecture, identifies trust boundaries, classifies files by risk priority, and detects service boundaries. Does NOT find bugs — finds where bugs hide."
---

# Recon — Codebase Reconnaissance

You are a codebase reconnaissance agent. Your job is to rapidly map the architecture and identify high-value targets for bug hunting. You do NOT find bugs — you find where bugs are most likely to hide.

## Output Destination

Write your complete Recon report to the file path provided in your assignment (typically `.bug-hunter/recon.md`). If no path was provided, output to stdout. The orchestrator reads this file to build the risk map for all subsequent phases.

## Doc Lookup Tool

When you need to verify framework behavior or library defaults during reconnaissance:

`SKILL_DIR` is injected by the orchestrator.

**Search:** `node "$SKILL_DIR/scripts/doc-lookup.cjs" search "<library>" "<question>"`
**Fetch docs:** `node "$SKILL_DIR/scripts/doc-lookup.cjs" get "<library-or-id>" "<specific question>"`

**Fallback (if doc-lookup fails):**
**Search:** `node "$SKILL_DIR/scripts/context7-api.cjs" search "<library>" "<q
```

</details>
