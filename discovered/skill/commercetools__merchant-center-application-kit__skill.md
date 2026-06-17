---
name: commercetools__merchant-center-application-kit__skill
source: https://github.com/commercetools/merchant-center-application-kit/blob/55662cfc5dd2683f844299c7a9890ad0e3f04950/.agents/skills/security-auditor/SKILL.md
repo: commercetools/merchant-center-application-kit
kind: skill
stars: 78
last_pushed: 2026-06-13T05:57:08Z
license: mit
score: 9
domains: [security, agents-ai, cli-tools]
tags: [audit, pentesting, devsecops]
curated: 2026-06-16
curated_by: config-scout
---

# commercetools/merchant-center-application-kit — skill

**Why it's worth keeping:** The agent includes exhaustive vulnerability categories (Injection, Auth, etc.) and enforces a strict reporting format including specific remediation code and exploit steps.

**Summary:** A sophisticated security auditing tool that uses structured taxonomies to identify vulnerabilities and generate functional proofs of concept.

**Source credibility:** High-quality enterprise source from commercetools with active maintenance.

**Recency:** Current; uses advanced task orchestration patterns for modern Claude Code instances.

**Source:** [commercetools/merchant-center-application-kit/.agents/skills/security-auditor/SKILL.md](https://github.com/commercetools/merchant-center-application-kit/blob/55662cfc5dd2683f844299c7a9890ad0e3f04950/.agents/skills/security-auditor/SKILL.md) · 78★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: security-auditor
description: Perform comprehensive security audit of a repository with detailed findings and step-by-step PoCs. Reports all web and API security vulnerabilities.
disable-model-invocation: false
argument-hint: '[--path <directory>] [--focus <category>]'
allowed-tools: Task, Bash, Grep, Glob, Read, Write
---

# Security Audit

Perform a comprehensive security audit of a repository, identifying web and API security vulnerabilities with practical exploitation steps and detailed proof-of-concept demonstrations.

## Arguments

- `--path <directory>` (optional): Path to the repository to audit. Defaults to current directory.
- `--focus <category>` (optional): Focus on specific security category (e.g., `injection`, `auth`, `api`, `crypto`, `logic`). Defaults to all categories.

## Process

### 1. Initialize Audit

Determine the audit scope and target directory:

```bash
# If --path is provided, use it; otherwise use current directory
TARGET_PATH=$(echo "$ARGUMENTS" | grep -oP '(?<=--path\s)\S+' || pwd)
FOCUS_AREA=$(echo "$ARGUMENTS" | grep -oP '(?<=--focus\s)\S+' || echo "all")
```

Create audit report filename with timestamp:

```bash
TIMESTAMP=$(date +%Y%m%d_%H
```

</details>
