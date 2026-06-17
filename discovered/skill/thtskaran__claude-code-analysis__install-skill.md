---
name: thtskaran__claude-code-analysis__install-skill
source: https://github.com/thtskaran/claude-code-analysis/blob/74a31c55fe56d4ea4f37813605a0558259377301/INSTALL-SKILL.md
repo: thtskaran/claude-code-analysis
kind: skill
stars: 120
last_pushed: 2026-04-02T10:03:22Z
license: other
score: 8
domains: [agents-ai, cli-tools, security, software-architecture]
tags: [audit, multi-pass, reasoning, expert-system]
curated: 2026-06-15
curated_by: config-scout
---

# thtskaran/claude-code-analysis — skill

**Why it's worth keeping:** The 'Recon -> Fetch Knowledge -> Re-read Code' pattern is a superior way to handle complex analysis; the file-based scratchpad provides excellent persistent memory for long-running reasoning tasks.

**Summary:** A multi-pass auditing skill that uses external production patterns to identify gaps in local implementations via an iterative ReAct loop.

**Source credibility:** High credibility due to significant social proof (120 stars) and specific reverse-engineering expertise.

**Recency:** Highly current, matching modern Claude Code tool use patterns.

**Source:** [thtskaran/claude-code-analysis/INSTALL-SKILL.md](https://github.com/thtskaran/claude-code-analysis/blob/74a31c55fe56d4ea4f37813605a0558259377301/INSTALL-SKILL.md) · 120★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Install: `/internals` Skill

A multi-pass deep audit skill. It reads your code, fetches Anthropic's production patterns, builds a scratchpad to think across passes, re-reads your code with new knowledge, follows chains across subsystems, and doesn't stop until every question is answered.

## Install

```bash
mkdir -p ~/.claude/skills/internals && curl -sL \
  https://raw.githubusercontent.com/thtskaran/claude-code-analysis/master/.claude/skills/internals/SKILL.md \
  -o ~/.claude/skills/internals/SKILL.md
```

That's it. Works across all your projects.

## How It Works

The skill runs a **multi-pass ReAct loop**, not a one-shot analysis:

![Skill ReAct Loop](infographics/skill-react-loop.svg)

**Pass 1 — Recon:** Fetches the live `TREE.md` index from GitHub. Reads your source files — not just the file you pointed at, but imports, callers, config, tests, error handling. Creates a scratchpad at `.claude/internals-scratchpad.md` with sections for subsystems, docs to fetch, gaps, open questions, and threads to pull.

**Pass 2 — First Fetch:** Pulls 2-4 primary Anthropic docs matched by topic tags. Reads them fully — critical patterns are buried deep. Extracts specifics to the scratch
```

</details>
