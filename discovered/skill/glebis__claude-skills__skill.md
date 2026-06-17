---
name: glebis__claude-skills__skill
source: https://github.com/glebis/claude-skills/blob/f47170dee300dd3d5da2a1c3c708986faeea3d5a/cognitive-toolkit/skill.md
repo: glebis/claude-skills
kind: skill
stars: 268
last_pushed: 2026-06-15T20:03:32Z
license: unknown
score: 9
domains: [agents-ai, cli-tools, wellness]
tags: [cbt, dbt, protocol-driven, structured-session]
curated: 2026-06-16
curated_by: config-scout
---

# glebis/claude-skills — skill

**Why it's worth keeping:** The pattern of separating core logic into reference files, the explicit 'Session Flow' for agentic behavior, and the sophisticated configuration of personality (pushback) are excellent templates.

**Summary:** A highly structured therapeutic framework implementing CBT/DBT protocols through command-driven workflows. It utilizes a modular reference system and manages session state via configurable 'pushback' levels.

**Source credibility:** High-quality repository with significant community interest indicated by star count.

**Recency:** Current; demonstrates advanced use of MCP integration and command-driven state management.

**Source:** [glebis/claude-skills/cognitive-toolkit/skill.md](https://github.com/glebis/claude-skills/blob/f47170dee300dd3d5da2a1c3c708986faeea3d5a/cognitive-toolkit/skill.md) · 268★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cognitive-toolkit
description: Evidence-based CBT and DBT intervention skills — guided thought records, opposite action, DEAR MAN roleplay, crisis skills with optional HRV biofeedback. Configurable therapeutic pushback. Triggers on "/cbt", "/dbt", "/thought-record", "/record", "/opposite", "/opposite-action", "I need to work through something", "help me with a thought", "cognitive distortion", "I'm spiraling", "can we do a thought record".
---

# Cognitive Toolkit

Interactive CBT and DBT guided exercises with configurable therapeutic pushback and optional health data integration.

## Usage

```
/cbt                        # start with check-in → technique recommendation
/cbt thought-record         # jump directly to thought record
/cbt opposite-action        # jump directly to opposite action
/cbt --pushback firm        # override pushback level for this session
/cbt --no-health            # skip health data pull even if available
```

## How it works

1. Read `references/thought-record.md` — thought record protocol (ABC model, cognitive distortion taxonomy, reframe scaffold)
2. Read `references/opposite-action.md` — opposite action + DEAR MAN + TIPP crisis skills
3. Rea
```

</details>
