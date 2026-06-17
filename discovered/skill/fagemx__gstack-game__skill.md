---
name: fagemx__gstack-game__skill
source: https://github.com/fagemx/gstack-game/blob/7259ab9782fa9c17e45c16f1fb8347823ddb4379/skills/spark-lens/SKILL.md
repo: fagemx/gstack-game
kind: skill
stars: 39
last_pushed: 2026-05-31T15:29:42Z
license: mit
score: 8
domains: [game-dev, agentic-workflows, cli-tools]
tags: [stateful, orchestration, creative-process]
curated: 2026-06-16
curated_by: config-scout
---

# fagemx/gstack-game — skill

**Why it's worth keeping:** The pattern of using a bash-based preamble to initialize environment variables, project directories, and shared artifact storage is an elite technique for creating persistent agentic workspaces. The prompt itself uses excellent 'Good vs Avoid' contrast examples to prevent the model from slipping into default corporate/analytical personas.

**Summary:** A highly sophisticated skill that integrates a heavy-duty shell preamble for state management, telemetry, and cross-session artifact persistence alongside high-quality creative prompting.

**Source credibility:** Specialized game production methodology (gstack) with growing community interest.

**Recency:** Highly current; demonstrates modern, advanced patterns for stateful CLI-based agents.

**Source:** [fagemx/gstack-game/skills/spark-lens/SKILL.md](https://github.com/fagemx/gstack-game/blob/7259ab9782fa9c17e45c16f1fb8347823ddb4379/skills/spark-lens/SKILL.md) · 39★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: spark-lens
description: "Low-pressure creative spark facilitation for early game ideas. Use when the user wants to protect enthusiasm, explore a half-formed concept, turn a feeling, image, character, mechanic, dream, or unfinished fragment into richer game possibilities, or leave an emotional imprint on the project before formal ideation/review. Avoid scoring, critique, feasibility checks, market language, investment language, pitch language, and forced deliverables."
user_invocable: true
preamble-tier: 1
---
<!-- AUTO-GENERATED from SKILL.md.tmpl — do not edit directly -->
<!-- Regenerate: bun scripts/gen-skill-docs.ts -->

## Preamble (run first)

```bash
setopt +o nomatch 2>/dev/null || true  # zsh compat
_GD_VERSION="0.5.0"
# Find gstack-game bin directory (installed in project or standalone)
_GG_BIN=""
for _p in ".claude/skills/gstack-game/bin" ".claude/skills/game-review/../../gstack-game/bin" "$(dirname "$(readlink -f .claude/skills/game-review/SKILL.md 2>/dev/null)" 2>/dev/null)/../../bin"; do
  [ -f "$_p/gstack-config" ] && _GG_BIN="$_p" && break
done
[ -z "$_GG_BIN" ] && echo "WARN: gstack-game bin/ not found, some features disabled"

# Project identification
_S
```

</details>
