---
name: DataDog__datadog-agent__skill
source: https://github.com/DataDog/datadog-agent/blob/d6ccac5be68edc940182fa6666b16cde7c4d1c3e/.claude/skills/explain-lading-config/SKILL.md
repo: DataDog/datadog-agent
kind: skill
stars: 3648
last_pushed: 2026-06-16T17:50:35Z
license: apache-2.0
score: 9
domains: [cli-tools, devops, testing]
tags: [workflow-automation, knowledge-grounding, token-optimization]
curated: 2026-06-16
curated_by: config-scout
---

# DataDog/datadog-agent — skill

**Why it's worth keeping:** It demonstrates expert patterns for tool-driven workflows: environment validation, sophisticated ambiguity handling via exit codes, and 'smart reading' strategies to optimize token usage on large files.

**Summary:** A highly specialized skill that automates the explanation of complex regression test configurations by grounding them in the underlying source code.

**Source credibility:** Very high; sourced from the Datadog Agent repository, a major industry-standard project.

**Recency:** 

**Source:** [DataDog/datadog-agent/.claude/skills/explain-lading-config/SKILL.md](https://github.com/DataDog/datadog-agent/blob/d6ccac5be68edc940182fa6666b16cde7c4d1c3e/.claude/skills/explain-lading-config/SKILL.md) · 3648★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: explain-lading-config
description: Explains a lading.yaml config file from the regression test suite, using the lading Rust source as ground truth for field meanings and defaults.
user_invocable: true
argument-hint: "[experiment name]"
---

# explain-lading-config

Explain what a lading regression test config does, grounded in lading source code.

## Quick Start

```bash
# 1. Verify the lading checkout exists and is on a known branch
bash .claude/skills/explain-lading-config/scripts/validate-lading-checkout.sh

# 2. Resolve $ARGUMENTS to a lading.yaml path (exact/substring/glob/path)
bash .claude/skills/explain-lading-config/scripts/resolve-lading-config.sh "$ARGUMENTS"

# 3. Read the resolved file, then ground every field in lading source
#    (see references/source-reading.md for the full strategy).

# 4. Write up the explanation following references/explanation-template.md.
```

Defaults must be resolved to concrete values, not function names. Full workflow below.

## Step 1: Validate lading checkout

Run `.claude/skills/explain-lading-config/scripts/validate-lading-checkout.sh`.

- Exit 0: script prints the current branch on stdout. If it is not `main`, warn
  the use
```

</details>
