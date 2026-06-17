---
name: ibalasite__getcost
source: https://github.com/ibalasite/getcost/blob/4cb2e1133efc35c857f9fa40d59b8cbbdcb35b89/skill.md
repo: ibalasite/getcost
kind: skill
stars: 0
last_pushed: 2026-05-02T22:09:11Z
license: unknown
score: 7
domains: [cli-tools, agents-ai]
tags: [cost-tracking, usage-metrics]
curated: 2026-06-15
curated_by: config-scout
---

# ibalasite/getcost — skill

**Why it's worth keeping:** Provides an excellent template for procedural orchestration: dependency guarding, argument mapping, and detailed error recovery instructions.

**Summary:** Tracks token usage and costs by wrapping a specific Python-based calculation script.

**Source credibility:** Low; zero stars and unknown license suggest a niche or unproven utility.

**Recency:** Current with Claude Code skill patterns.

**Source:** [ibalasite/getcost/skill.md](https://github.com/ibalasite/getcost/blob/4cb2e1133efc35c857f9fa40d59b8cbbdcb35b89/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: getcost
description: |
  Show Claude Code token usage and costs for the current project directory.
  Reports current session spend and all-time directory total in USD + local currency.
  Use when the user invokes /getcost or asks about token costs, spending, or usage.
allowed-tools:
  - Bash
---

# /getcost — Token Cost Report

Show token usage and costs for the current project.

---

## Step 1 — Guard: runtime installed?

```bash
test -f "$HOME/.claude/skills/getcost/bin/getcost-calc.py"
```

**[AI 指令]** If not found, output:

```
[getcost] Not installed. Run:
  git clone https://github.com/ibalasite/getcost.git ~/.claude/skills/getcost
  ~/.claude/skills/getcost/setup install
```

Then stop.

---

## Step 2 — Parse argument

Check if user passed `all` as an argument (e.g. `/getcost all`).

```bash
# _ARG is "all" if user wrote "/getcost all", otherwise empty
_ARG=""
```

---

## Step 3 — Run report

```bash
python3 "$HOME/.claude/skills/getcost/bin/getcost-calc.py" \
  --report \
  --cwd "$PWD" \
  ${_ARG:+--all}
```

**[AI 指令]** Run via Bash tool. Display the full output verbatim to the user. Do not summarise or reformat.

---

## Step 4 — Error handling

If the script
```

</details>
