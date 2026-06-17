---
name: semgrep__skills__skill
source: https://github.com/semgrep/skills/blob/90cc990a535098a84950b18d8cf770e097da1c77/skills/code-security/SKILL.md
repo: semgrep/skills
kind: skill
stars: 227
last_pushed: 2026-06-08T08:24:41Z
license: other
score: 9
domains: [security, devops, backend]
tags: [security-audit, owasp, threat-modeling, proactive-review]
curated: 2026-06-15
curated_by: config-scout
---

# semgrep/skills — skill

**Why it's worth keeping:** The 'Proactive mode' instruction forces the agent to intercept dangerous patterns without being asked, while the impact-based hierarchy (Critical/High) creates a clear triage system. The inclusion of language-specific vulnerability priorities is highly effective for steering LLM attention.

**Summary:** A comprehensive security auditing framework that instructs the agent to perform proactive vulnerability scans during standard coding tasks. It categorizes risks by impact and provides language-specific priority lists for efficient reasoning.

**Source credibility:** Highly credible; Semgrep is an industry leader in static analysis and security tooling.

**Recency:** Current; uses advanced agentic patterns like proactive/reactive modes suited for Claude Code.

**Source:** [semgrep/skills/skills/code-security/SKILL.md](https://github.com/semgrep/skills/blob/90cc990a535098a84950b18d8cf770e097da1c77/skills/code-security/SKILL.md) · 227★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: code-security
description: "Security guidelines for writing secure code. Use when writing code, reviewing code for vulnerabilities, or asking about secure coding practices like 'check for SQL injection' or 'review security'. IMPORTANT: Always consult this skill when writing or reviewing any code that handles user input, authentication, file operations, database queries, network requests, cryptography, or infrastructure configuration (Terraform, Kubernetes, Docker, GitHub Actions) — even if the user doesn't explicitly mention security. Also use when users ask to 'review my code', 'check this for bugs', or 'is this safe'."
---

# Code Security Guidelines

Comprehensive security rules for writing secure code across 15+ languages. Covers OWASP Top 10, infrastructure security, and coding best practices with 28 rule categories.

## How to Use This Skill

**Proactive mode** — When writing or reviewing code, automatically check for relevant vulnerabilities based on the language and patterns present. You don't need to wait for the user to ask about security.

**Reactive mode** — When the user asks about security, use the categories below to find the relevant rule file, then read i
```

</details>
