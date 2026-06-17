---
name: genecyber__loadout__audit-skill
source: https://github.com/genecyber/loadout/blob/e3717f78caa4b32cece3e54e241ab6b2ddcf8854/prompts/audit-skill.md
repo: genecyber/loadout
kind: skill
stars: 0
last_pushed: 2026-01-29T09:45:38Z
license: unknown
score: 8
domains: [security, agents-ai, devops]
tags: [security-audit, protocol, safety]
curated: 2026-06-16
curated_by: config-scout
---

# genecyber/loadout — skill

**Why it's worth keeping:** It provides a highly specific checklist of technical red flags (like shell injection patterns) and a standardized risk-level reporting structure.

**Summary:** A systematic security auditing protocol that guides an AI agent through verifying script safety, metadata accuracy, and potential vulnerabilities.

**Source credibility:** Low based on repository metrics (0 stars), but the content demonstrates high professional security standards.

**Recency:** Current; the methodology is highly applicable to modern agentic workflows and file-system interactions.

**Source:** [genecyber/loadout/prompts/audit-skill.md](https://github.com/genecyber/loadout/blob/e3717f78caa4b32cece3e54e241ab6b2ddcf8854/prompts/audit-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Security Audit Guide Template

This guide provides a structured approach for analyzing skill security and identifying potential vulnerabilities.

## Overview

When auditing a skill, you are performing a comprehensive security review to ensure it is safe to use. This includes analyzing scripts, verifying frontmatter claims, assessing trust levels, and flagging suspicious patterns.

## Skill Information to Gather

Before beginning the audit, collect the following information:

- **Name**: The skill's identifier
- **Description**: What the skill claims to do
- **Path**: Location of the skill directory
- **SKILL.md Path**: Location of the main skill file
- **Author**: Who created the skill (if specified)
- **Version**: Current version (if specified)
- **License**: License type (if specified)

## Audit Checklist

### 1. Script Analysis

For each script in the `scripts/` directory, perform the following checks:

- [ ] **Shell Injection Vulnerabilities**
  - Look for unescaped variables in shell commands
  - Check for `eval` usage with user input
  - Identify `$()` or backtick command substitution with untrusted data
  - Search for `source` or `.` commands with dynamic paths

- [ ] **Ne
```

</details>
