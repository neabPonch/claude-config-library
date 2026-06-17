---
name: openbashok__promptzero__skill
source: https://github.com/openbashok/promptzero/blob/b6869ac06dd05f971fe1270b5d160e63ea99bc23/agents/skill.md
repo: openbashok/promptzero
kind: skill
stars: 60
last_pushed: 2026-05-18T13:37:43Z
license: unknown
score: 9
domains: [security, agents-ai, privacy]
tags: [pii-anonymization, data-privacy, security-pattern]
curated: 2026-06-15
curated_by: config-scout
---

# openbashok/promptzero — skill

**Why it's worth keeping:** The bidirectional mapping logic and specific synthetic data replacement templates provide a perfect blueprint for building secure agentic workflows.

**Summary:** A technical specification for a 'detect-replace-restore' algorithm to anonymize PII before LLM communication.

**Source credibility:** High; authored by security professionals with an active, well-regarded repository.

**Recency:** Current; updated within the last month.

**Source:** [openbashok/promptzero/agents/skill.md](https://github.com/openbashok/promptzero/blob/b6869ac06dd05f971fe1270b5d160e63ea99bc23/agents/skill.md) · 60★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skill: PII-Safe LLM Communication (PromptZero Methodology)

**Skill ID:** `promptzero-pii-safe-llm`
**Version:** 2.3.0
**Source:** https://github.com/openbashok/promptzero
**Author:** OpenBash.com — from pentesters, to pentesters

---

## Purpose

This skill enables an agent to:
1. Recognize when a prompt or workflow contains sensitive data that must not reach an external LLM
2. Apply the PromptZero anonymization methodology (detect → replace → forward → restore)
3. Help users and developers implement PII-safe LLM integrations
4. Build or recommend systems where real data never leaves the local environment

---

## When to Activate This Skill

Activate when the user or task involves any of:
- Sending prompts to an LLM that contain IPs, hostnames, credentials, or personal data
- Building an AI integration for a security, healthcare, legal, or financial context
- Implementing an agent or pipeline that processes sensitive documents
- Pentesting workflows where infrastructure details must not reach external APIs
- Any scenario where GDPR, HIPAA, PCI-DSS, or data residency regulations apply
- A user asks about "privacy", "anonymization", "PII", "data leakage" in AI context

---

## Co
```

</details>
