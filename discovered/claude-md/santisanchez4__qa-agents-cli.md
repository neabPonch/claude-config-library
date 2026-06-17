---
name: santisanchez4__qa-agents-cli
source: https://github.com/santisanchez4/qa-agents-cli/blob/d9e8f676a310cdb73f0568f1bb16f0451445530e/CLAUDE.md
repo: santisanchez4/qa-agents-cli
kind: claude-md
stars: 0
last_pushed: 2026-05-31T02:43:28Z
license: unknown
score: 8
domains: [cli-tools, qa-automation]
tags: [cli, architecture, automation, decoupling]
curated: 2026-06-14
curated_by: config-scout
---

# santisanchez4/qa-agents-cli — claude-md

**Why it's worth keeping:** It defines a 'Generic product rule' to prevent LLM-driven hardcoding of project-specific logic; it provides precise command signatures including nuanced flag interaction rules (e.g., dry-run priority).

**Summary:** A technical blueprint for a generic QA automation CLI that enforces strict decoupling between the tool and its target repositories.

**Source credibility:** Low visibility/stars, but the content demonstrates advanced architectural discipline.

**Recency:** Current; reflects modern CLI development patterns.

**Source:** [santisanchez4/qa-agents-cli/CLAUDE.md](https://github.com/santisanchez4/qa-agents-cli/blob/d9e8f676a310cdb73f0568f1bb16f0451445530e/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# QA Agents CLI - Project Memory

## Project goal

This repo is a local CLI tool called `qa-agents-cli`.

The goal is to build a reusable QA Automation Agent Stack that can be used locally against any automation project.

---

## Generic product rule

`qa-agents-cli` is the reusable engine.

It must not hardcode project names, folder structures, business rules, URLs, credentials, or any project-specific concepts (including anything Warzone-specific).

Target repositories provide local context through:

```txt
<target-repo>/.qa-agents/project-profile.json
<target-repo>/.qa-agents/repo-rules.md
<target-repo>/.qa-agents/execution-config.json
<target-repo>/.qa-agents/specs/
<target-repo>/.qa-agents/runs/
```

Any behavior discovered during lab testing must be generalized before being added to the CLI logic. If it only makes sense for one project, it belongs in that project's `.qa-agents/` files — not here.

---

## Lab projects

`warzone-ui` is used only to validate the CLI against a real project. It is a laboratory, not a built-in or default target. The CLI must work equally well against any repo with a compatible structure.

Warzone-specific rules live exclusively in:

```txt
C:\Repo
```

</details>
