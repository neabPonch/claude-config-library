---
name: jensabrahamsson__overblick
source: https://github.com/jensabrahamsson/overblick/blob/715f85c1f4e3ffdde618c751f1682db5f22822e1/CLAUDE.md
repo: jensabrahamsson/overblick
kind: claude-md
stars: 2
last_pushed: 2026-05-14T15:09:43Z
license: gpl-3.0
score: 8
domains: [agents-ai, security, cli-tools]
tags: [architectural-mapping, strict-constraints, agentic-framework]
curated: 2026-06-16
curated_by: config-scout
---

# jensabrahamsson/overblick — claude-md

**Why it's worth keeping:** Uses highly structured classification tables to map system capabilities and employs 'CRITICAL' instruction blocks to prevent specific, high-risk developer errors like identity mismatches or network lockouts.

**Summary:** Provides comprehensive architectural mapping and strict operational constraints for a multi-agent framework.

**Source credibility:** The depth of detail suggests a sophisticated, functional codebase despite the low star count.

**Recency:** Highly current, with activity within the last month.

**Source:** [jensabrahamsson/overblick/CLAUDE.md](https://github.com/jensabrahamsson/overblick/blob/715f85c1f4e3ffdde618c751f1682db5f22822e1/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Överblick Agent Framework

## Git Identity — CRITICAL
**The git author for this repo is `Jens Abrahamsson <jens.abrahamsson@makeitso.se>`.**
NEVER commit with any other identity. Before committing, ALWAYS verify:
```bash
git config user.name   # Must be "Jens Abrahamsson"
git config user.email  # Must be "jens.abrahamsson@makeitso.se"
```
If these are wrong, fix them BEFORE committing:
```bash
git config user.name "Jens Abrahamsson"
git config user.email "jens.abrahamsson@makeitso.se"
```
**DO NOT** use any other name or email. Wrong git identity has caused history rewrites before and is treated as a serious incident.

## Quality Standard
**PERFECTION IS THE STANDARD.** Every file, every test, every prompt, every line of code must be production-grade. No shortcuts. No "good enough." No TODO comments left behind. If it's worth building, it's worth building right.

## Overview
Överblick is a security-focused multi-identity agent framework with a personality stable. It consolidates multiple agent personalities (Anomal, Cherry, Blixt, Björk, Prisma, Rost, Natt, Stål, Smed, PolyTrader, Vakt) plus a special Supervisor system identity into ONE codebase with a plugin architec
```

</details>
