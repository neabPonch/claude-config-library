---
name: claude-code-best__claude-code__skill
source: https://github.com/claude-code-best/claude-code/blob/ddf1acdaedfef5e81af5c99bf8273fc86a84bae9/.claude/skills/teach-me/SKILL.md
repo: claude-code-best/claude-code
kind: skill
stars: 19989
last_pushed: 2026-06-15T11:09:50Z
license: unknown
score: 9
domains: [education, learning-management]
tags: [tutor, pedagogy, state-management, interactive]
curated: 2026-06-15
curated_by: config-scout
---

# claude-code-best/claude-code — skill

**Why it's worth keeping:** It utilizes AskUserQuestion as a cognitive scaffold rather than just a UI tool and implements a robust local state system for long-term session resumption.

**Summary:** A sophisticated pedagogical agent that uses structured dialogue and file-based persistence to teach topics through progressive concept mastery.

**Source credibility:** High-star, high-activity repository indicating a highly vetted or community-driven collection.

**Recency:** Current; uses modern Claude Code patterns like structured AskUserQuestion options and file-based state management.

**Source:** [claude-code-best/claude-code/.claude/skills/teach-me/SKILL.md](https://github.com/claude-code-best/claude-code/blob/ddf1acdaedfef5e81af5c99bf8273fc86a84bae9/.claude/skills/teach-me/SKILL.md) · 19989★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: teach-me
description: "Personalized 1-on-1 AI tutor. Diagnoses level, builds learning path, teaches via guided questions, tracks misconceptions. Use when user wants to learn/study/understand a topic, says 'teach me', 'help me understand', or invokes /teach-me."
---

# Teach Me

Personalized mastery tutor. Diagnose, question, advance on understanding.

## Usage

```bash
/teach-me Python decorators
/teach-me 量子力学 --level beginner
/teach-me React hooks --resume
```

## Arguments

| Argument | Description |
|----------|-------------|
| `<topic>` | Subject to learn (required, or prompted) |
| `--level <level>` | Starting level: beginner, intermediate, advanced (default: diagnose) |
| `--resume` | Resume previous session from `.claude/skills/teach-me/records/{topic-slug}/` |

## Core Rules

1. **Minimize lecturing, but don't be dogmatic.** Prefer questions that lead to discovery. For complete beginners with zero context, a brief 1-2 sentence framing is acceptable before asking.
2. **Diagnose first.** Always probe current understanding before teaching.
3. **Mastery gate.** Advance to next concept only when the learner can explain it clearly and apply it.
4. **1-2 questions per r
```

</details>
