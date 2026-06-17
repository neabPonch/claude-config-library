---
name: sigridjineth__hello-ansible-skills__skill
source: https://github.com/sigridjineth/hello-ansible-skills/blob/3062baada51d4fb2279334a7e8bf3e7d02347fde/skills/ansible-debug/SKILL.md
repo: sigridjineth/hello-ansible-skills
kind: skill
stars: 65
last_pushed: 2026-01-17T12:22:10Z
license: mit
score: 7
domains: [devops, infrastructure-automation, cli-tools]
tags: [ansible, troubleshooting, debugging]
curated: 2026-06-15
curated_by: config-scout
---

# sigridjineth/hello-ansible-skills — skill

**Why it's worth keeping:** The categorization-to-diagnosis mapping and specific command suggestions (like connectivity tests and verbosity levels) provide an agent with a clear mental model for debugging infrastructure.

**Summary:** Provides a structured troubleshooting framework for Ansible errors by categorizing them into connection, authentication, module, and syntax issues.

**Source credibility:** Decent; the repo has specialized interest indicated by its star count for a niche toolset.

**Recency:** Current; Ansible best practices for debugging remain stable.

**Source:** [sigridjineth/hello-ansible-skills/skills/ansible-debug/SKILL.md](https://github.com/sigridjineth/hello-ansible-skills/blob/3062baada51d4fb2279334a7e8bf3e7d02347fde/skills/ansible-debug/SKILL.md) · 65★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ansible-debug
description: Use when playbooks fail with UNREACHABLE, permission denied, MODULE FAILURE, or undefined variable errors. Use when SSH connections fail or sudo password is missing.
---

# Ansible Debugging

## Overview

Ansible errors fall into four categories: connection, authentication, module, and syntax. Systematic diagnosis starts with identifying the category, then isolating the specific cause.

## When to Use

- UNREACHABLE errors (SSH/network issues)
- Permission denied or sudo password errors
- MODULE FAILURE messages
- Undefined variable errors
- Template rendering failures
- Slow playbook execution

## Error Categories

| Category | Symptoms | First Check |
|----------|----------|-------------|
| Connection | UNREACHABLE | `ssh -v user@host` |
| Authentication | Permission denied, Missing sudo password | SSH keys, sudoers config |
| Module | MODULE FAILURE | Module parameters, target state |
| Syntax | YAML parse error | Line number in error, indentation |

## Quick Diagnosis

### Connection Errors

```bash
# Test SSH directly
ssh -v -i /path/to/key user@hostname

# Test port connectivity
nc -zv hostname 22

# Verify inventory parsing
ansible-invent
```

</details>
