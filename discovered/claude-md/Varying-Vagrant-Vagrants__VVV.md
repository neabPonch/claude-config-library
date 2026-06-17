---
name: Varying-Vagrant-Vagrants__VVV
source: https://github.com/Varying-Vagrant-Vagrants/VVV/blob/8c7a42c1a35d23b1bef3efd7035488973f68324a/CLAUDE.md
repo: Varying-Vagrant-Vagrants/VVV
kind: claude-md
stars: 4525
last_pushed: 2026-06-08T10:43:10Z
license: mit
score: 9
domains: [devops, infrastructure-as-code, wordpress, dev-environment]
tags: [guardrails, git-safety, workflow-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# Varying-Vagrant-Vagrants/VVV — claude-md

**Why it's worth keeping:** Uses highly effective 'scenario modeling' and 'correct/incorrect' examples; includes a mandatory pre-commit verification checklist that an agent can execute before performing actions.

**Summary:** Establishes strict architectural boundaries between infrastructure code and user-generated site content to prevent accidental commits of ephemeral data. Uses 'Correct vs Incorrect' pattern matching to guide agent behavior.

**Source credibility:** High (4,500+ stars and actively maintained repository).

**Recency:** Very current; specifically designed for tool-using agents capable of complex file/git operations.

**Source:** [Varying-Vagrant-Vagrants/VVV/CLAUDE.md](https://github.com/Varying-Vagrant-Vagrants/VVV/blob/8c7a42c1a35d23b1bef3efd7035488973f68324a/CLAUDE.md) · 4525★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# VVV Development Environment Instructions for LLM Agents

This document provides critical guidance for AI coding assistants working with Varying Vagrant Vagrants (VVV). **Read and follow these instructions carefully to avoid inappropriate changes.**

## 🚨 Critical Boundaries - NEVER Cross These Lines

### DO NOT Modify These Core Files
- **`.gitignore`** - NEVER modify to allow committing `www/` content or other gitignored paths
- **`Vagrantfile`** - Core Vagrant configuration, do not modify without explicit permission
- **`/provision/`** scripts - Core provisioning logic (only modify for VVV improvements, not site work)
- **Git-tracked files** - Assume files tracked by git are VVV core files unless explicitly told otherwise

### Git Safety Rules - Follow These Strictly
1. **NEVER modify `.gitignore`** to allow committing `www/` content
2. **NEVER force commit** using `--no-verify`, `-f`, or similar flags
3. **ALWAYS check `git check-ignore <path>`** before committing files to verify they should be tracked
4. **If files in `www/` appear in git status** - they should almost certainly NOT be committed (except the defaults listed below)
5. **Ask before committing** if you're uncertai
```

</details>
