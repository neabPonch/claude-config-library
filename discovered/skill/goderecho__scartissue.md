---
name: goderecho__scartissue
source: https://github.com/goderecho/scartissue/blob/980b2ea342c021c6f7f979124045f5dc74d849ce/skill.md
repo: goderecho/scartissue
kind: skill
stars: 0
last_pushed: 2026-05-06T20:49:02Z
license: unknown
score: 7
domains: [cli-tools, devops, quality-assurance]
tags: [git, diff-analysis, regression-detection]
curated: 2026-06-14
curated_by: config-scout
---

# goderecho/scartissue — skill

**Why it's worth keeping:** Excellent pattern of instructing the agent to explain 'why' a missing file matters rather than just listing it, plus providing proactive follow-up suggestions.

**Summary:** Provides instructions for an agent to use an external 'Scar Tissue' database to analyze git diffs for historical co-change patterns and potential regression gaps.

**Source credibility:** Low social proof (0 stars) and likely an internal tool for a specific company (Salesbricks).

**Recency:** Current; utilizes standard git workflows highly compatible with modern CLI agents.

**Source:** [goderecho/scartissue/skill.md](https://github.com/goderecho/scartissue/blob/980b2ea342c021c6f7f979124045f5dc74d849ce/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: scartissue
description: Run the Scar Tissue co-change analyzer against the current branch diff and surface hot files, co-change gaps, and relevant checklists.
---

Scar Tissue is a knowledge base of 827 historical Salesbricks bugs at `__SCARTISSUE_PATH__`. Use it to surface what's risky about the current diff — not just what's IN the diff, but what's conspicuously ABSENT.

## What to do when invoked

### Step 1 — Check Scar Tissue is available

```bash
ls __SCARTISSUE_PATH__/tools/analyze.py 2>/dev/null && echo "found" || echo "missing"
```

If missing, tell the user:
> "Scar Tissue not found. Run: `git clone git@github.com:goderecho/scartissue.git <path> && <path>/install.sh`"

### Step 2 — Run the analyzer against the current repo

```bash
git diff production...HEAD --name-only | python3 __SCARTISSUE_PATH__/tools/analyze.py --stdin
```

**Variations based on args:**
- `args: staged` → staged files only:
  ```bash
  git diff --cached --name-only | python3 __SCARTISSUE_PATH__/tools/analyze.py --stdin
  ```
- `args: SAL-XXXX` → look up a specific case:
  ```bash
  cat __SCARTISSUE_PATH__/cases/SAL-XXXX.md
  ```
- No args → uses `git diff production...HEAD` automatically:
```

</details>
