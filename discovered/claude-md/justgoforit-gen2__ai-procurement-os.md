---
name: justgoforit-gen2__ai-procurement-os
source: https://github.com/justgoforit-gen2/ai-procurement-os/blob/80b66b54791ee9ca629e2bf41faeaee5e3abfcf6/claude.md
repo: justgoforit-gen2/ai-procurement-os
kind: claude-md
stars: 1
last_pushed: 2026-04-19T22:54:14Z
license: unknown
score: 8
domains: [backend-api, security, architecture]
tags: [rule-enforcement, modular-design, data-governance]
curated: 2026-06-16
curated_by: config-scout
---

# justgoforit-gen2/ai-procurement-os — claude-md

**Why it's worth keeping:** It uses 'non-negotiable rules' to prevent destructive file actions and provides a high-density 'Source of Truth' map to minimize context-loading errors.

**Summary:** Provides rigorous architectural guardrails for a modular procurement platform, focusing on data lifecycle, security-first audit logging, and feature toggling.

**Source credibility:** Low social proof via GitHub stars, but the depth of technical constraint suggests a real-world engineering project.

**Recency:** Current; utilizes modern patterns for config-driven development suitable for agentic coding.

**Source:** [justgoforit-gen2/ai-procurement-os/claude.md](https://github.com/justgoforit-gen2/ai-procurement-os/blob/80b66b54791ee9ca629e2bf41faeaee5e3abfcf6/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Procurement OS (A) — Claude Code Instructions

## Goal
Build a modular procurement platform.
POC uses Streamlit UI; product delivery is FastAPI "kits" (Standard/Expansion/Automation/Full).

## Non-negotiable rules
- Persist any input or output file with split storage:
  - SQL DB stores metadata only.
  - secure_store/ stores original files.
- File retention period is 7 years.
- After 7 years, perform deletion confirmation and let a human make the final decision.
- Do NOT delete any file without explicit human approval.
- Audit logs must store METADATA ONLY (request_id, timestamps, hash, status, counts, versions).
- Keep entrypoints thin:
  - Streamlit: apps/*/app.py
  - FastAPI: services/api/main.py
- Put business logic in packages/proc_core/.
- Runtime behavior is config-driven (config/*.yaml). Skills markdown is design-time only.

## Where to look (source of truth)
- Latest assumptions & constraints: docs/CONTEXT.md
- Security policy: docs/runbook/security.md
- Runtime configs: config/
- Canonical schemas: schemas/
- Core code: packages/proc_core/
- API routes: services/api/routes/
- UI apps: apps/

## Kits (module toggles)
- Standard Kit: spend
- Expansion Kit: spend + rfx
- A
```

</details>
