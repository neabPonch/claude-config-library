---
name: Benn25__handrail
source: https://github.com/Benn25/handrail/blob/6c3631cf5f766ecef43f1a5344092ec3c32cc6da/CLAUDE.md
repo: Benn25/handrail
kind: claude-md
stars: 12
last_pushed: 2026-05-24T07:02:40Z
license: unknown
score: 8
domains: [cli-tools, workflow-automation]
tags: [session-init, structural-rules, git-management]
curated: 2026-06-15
curated_by: config-scout
---

# Benn25/handrail — claude-md

**Why it's worth keeping:** The mandatory session-start structure check is an excellent guardrail against agentic mistakes. The conditional refactoring logic (the 500-line rule) offers a predictable way to manage project scale without manual oversight.

**Summary:** Establishes a strict 'Review -> Suggest -> Approve' protocol at session start to prevent file drift and provides automated architectural rules based on line-count thresholds.

**Source credibility:** Small personal repo with highly specific, non-generic instructions.

**Recency:** Very current; it optimizes for the agency of modern tools that can execute terminal commands and Git operations directly.

**Source:** [Benn25/handrail/CLAUDE.md](https://github.com/Benn25/handrail/blob/6c3631cf5f766ecef43f1a5344092ec3c32cc6da/CLAUDE.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project: BlenderCLIrender
A Blender addon for batch rendering via command line launcher.

# My Working Preferences

## Who I am
- No command line experience — I do not use terminal commands myself
- I work across devices (PC, phone, browser)
- I have experience writing Arduino code and Blender addons, but in a basic/dirty way

## How I want Claude to work

### Git & GitHub
- Claude handles ALL git operations (commit, push, branch, etc.)
- I only do one thing on GitHub: click the banner → Create pull request → Merge
- Every logical change must be its own separate commit so I can accept or reject changes individually
- Never bundle unrelated changes into one commit

### File structure — mandatory on every session start
- At the start of every session, review the project file structure
- Identify what type of project it is (Blender addon, Arduino, etc.)
- Suggest what a standard/clean file structure should look like for that project type
- Wait for my explicit approval before moving, renaming, or creating any files

### Blender addon file structure rules
- Single file, under 500 lines → keep as one `.py` file, no folder, keep the addon name as the filename
- Single file, over 500 li
```

</details>
