---
name: szaghi__FoBiS__claude-skill
source: https://github.com/szaghi/FoBiS/blob/033a55730d60fdd4b32f71dd5b7d98579f1b40a1/docs/guide/claude-skill.md
repo: szaghi/FoBiS
kind: skill
stars: 143
last_pushed: 2026-05-12T06:27:36Z
license: unknown
score: 8
domains: [cli-tools, devops, fortran]
tags: [build-system, expert-knowledge, compiler-config]
curated: 2026-06-15
curated_by: config-scout
---

# szaghi/FoBiS — skill

**Why it's worth keeping:** The structure demonstrates how to include high-density technical specs like error diagnosis decision trees and JSON schemas to move beyond simple instruction into expert reasoning.

**Summary:** Provides deep domain expertise for the FoBiS Fortran build system, covering CLI commands, compilers, and dependency management.

**Source credibility:** Niche tool with moderate community interest (143 stars) and recent maintenance.

**Recency:** Current; specifically designed for the Claude Code skill architecture.

**Source:** [szaghi/FoBiS/docs/guide/claude-skill.md](https://github.com/szaghi/FoBiS/blob/033a55730d60fdd4b32f71dd5b7d98579f1b40a1/docs/guide/claude-skill.md) · 143★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Skill

FoBiS.py ships a [Claude Code](https://claude.ai/claude-code) skill that turns Claude into an expert FoBiS.py assistant. Install it once and Claude can answer questions, write `fobos` files, diagnose build errors, and help with every feature — without you needing to look up the documentation.

## Installation

The skill lives at `~/.claude/skills/fobis/SKILL.md`. Clone it:

```bash
mkdir -p ~/.claude/skills/fobis
curl -sSL https://raw.githubusercontent.com/szaghi/FoBiS/master/.claude/skills/fobis/SKILL.md \
  -o ~/.claude/skills/fobis/SKILL.md
```

Or copy it manually from the repository root:

```bash
cp /path/to/FoBiS/.claude/skills/fobis/SKILL.md ~/.claude/skills/fobis/SKILL.md
```

## Using the skill

Once installed, simply invoke it with `/fobis` in any Claude Code session:

```
/fobis write a fobos file for my project with debug and release modes
```

```
/fobis my build fails with "Module 'utils' not found" — how do I debug this?
```

```
/fobis how do I add PENF as a GitHub dependency?
```

```
/fobis show me a CI script that uses fobis build --json
```

Claude also auto-triggers the skill for questions that mention `fobos`, `FoBiS`, or Fortran build co
```

</details>
