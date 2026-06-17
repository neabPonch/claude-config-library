---
name: getsentry__sentry-python__skill
source: https://github.com/getsentry/sentry-python/blob/cc802f6fcedcbd50f76afe2fc902d4d21b6691d6/.agents/skills/skill-scanner/SKILL.md
repo: getsentry/sentry-python
kind: skill
stars: 2192
last_pushed: 2026-06-15T05:08:06Z
license: mit
score: 9
domains: [security, agents-ai]
tags: [audit, security-scan, prompt-injection, safety]
curated: 2026-06-15
curated_by: config-scout
---

# getsentry/sentry-python — skill

**Why it's worth keeping:** It provides a highly structured reasoning chain (Phases 1-8) that moves from automated static analysis to nuanced behavioral/intent evaluation, specifically addressing advanced risks like configuration poisoning and tool permission justification.

**Summary:** A sophisticated multi-phase security auditing framework designed to detect malicious intent, prompt injection, and privilege escalation in agent skills.

**Source credibility:** Highly professional; the logic mirrors industry-standard security audit workflows.

**Recency:** Current; incorporates modern Python tooling (uv) and specific Claude Code ecosystem file targets.

**Source:** [getsentry/sentry-python/.agents/skills/skill-scanner/SKILL.md](https://github.com/getsentry/sentry-python/blob/cc802f6fcedcbd50f76afe2fc902d4d21b6691d6/.agents/skills/skill-scanner/SKILL.md) · 2192★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: skill-scanner
description: Scan agent skills for security issues. Use when asked to "scan a skill",
  "audit a skill", "review skill security", "check skill for injection", "validate SKILL.md",
  or assess whether an agent skill is safe to install. Checks for prompt injection,
  malicious scripts, excessive permissions, secret exposure, and supply chain risks.
allowed-tools: Read, Grep, Glob, Bash
---

# Skill Security Scanner

Scan agent skills for security issues before adoption. Detects prompt injection, malicious code, excessive permissions, secret exposure, and supply chain risks.

**Important**: Run all scripts from the repository root using the full path via `${CLAUDE_SKILL_ROOT}`.

## Bundled Script

### `scripts/scan_skill.py`

Static analysis scanner that detects deterministic patterns. Outputs structured JSON.

```bash
uv run ${CLAUDE_SKILL_ROOT}/scripts/scan_skill.py <skill-directory>
```

Returns JSON with findings, URLs, structure info, and severity counts. The script catches patterns mechanically — your job is to evaluate intent and filter false positives.

## Workflow

### Phase 1: Input & Discovery

Determine the scan target:

- If the user provides a ski
```

</details>
