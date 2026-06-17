---
name: Cydiar__skill-guard__skill
source: https://github.com/Cydiar/skill-guard/blob/f2cc6cfc316966f7f058c51d81fc290865bb3d9d/skill/skill.md
repo: Cydiar/skill-guard
kind: skill
stars: 5
last_pushed: 2026-05-20T08:51:11Z
license: mit
score: 7
domains: [security, agents-ai, cli-tools]
tags: [security-audit, prompt-injection, cost-estimation]
curated: 2026-06-14
curated_by: config-scout
---

# Cydiar/skill-guard — skill

**Why it's worth keeping:** Provides a concrete CLI-driven workflow for validating the safety and efficiency of external agent tools via URLs.

**Summary:** A security auditing tool designed to scan AI agent skills for vulnerabilities, prompt injection risks, and token cost estimates.

**Source credibility:** Low star count but highly specialized niche with recent maintenance (1 month ago).

**Recency:** Current; updated very recently in relation to modern AI agent development.

**Source:** [Cydiar/skill-guard/skill/skill.md](https://github.com/Cydiar/skill-guard/blob/f2cc6cfc316966f7f058c51d81fc290865bb3d9d/skill/skill.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SkillGuard Security Audit

Audit AI Agent Skills for security vulnerabilities, prompt injection risks, and cost estimation.

## Description

SkillGuard performs comprehensive security audits on Claude Code Skills and other AI Agent plugins. It analyzes 10 security dimensions with 109 detection rules, providing detailed reports with risk scores and remediation guidance.

## Usage

When a user wants to audit a skill, ask for the GitHub or ClawHub URL, then run the audit script.

Example:
- "Audit this skill: https://github.com/user/my-skill"
- "Check security of https://clawhub.ai/author/skill-name"

## Commands

```bash
python3 skill/audit.py <github_or_clawhub_url>
```

The script will:
1. Submit the URL to SkillGuard API
2. Monitor scan progress
3. Display the security report in terminal

## Output

The audit provides:
- Overall security grade (A-F)
- Risk breakdown by dimension
- Detailed findings with severity levels
- Token cost estimates
- Remediation recommendations
```

</details>
