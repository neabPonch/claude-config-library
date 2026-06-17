---
name: hookdeck__webhook-skills__generate-skill
source: https://github.com/hookdeck/webhook-skills/blob/da37fc751d55f042ca4eaacb48b0c37ae54b66e0/scripts/skill-generator/prompts/generate-skill.md
repo: hookdeck/webhook-skills
kind: skill
stars: 73
last_pushed: 2026-06-07T09:02:26Z
license: mit
score: 9
domains: [backend-api, security, agents-ai, devops]
tags: [webhooks, meta-template, integration-patterns, verification]
curated: 2026-06-16
curated_by: config-scout
---

# hookdeck/webhook-skills — skill

**Why it's worth keeping:** It enforces a 'research-first' workflow for signature verification and mandates strict cross-file consistency to prevent documentation/code drift. It also includes high-value patterns like raw body handling, multi-framework examples (Node/Python), and local development CLI instructions.

**Summary:** A high-fidelity meta-template that instructs agents to generate multi-framework webhook integration skills with rigorous verification, consistency checks, and automated testing.

**Source credibility:** High; maintained by Hookdeck, a professional webhook infrastructure provider with active maintenance.

**Recency:** Current; specifically optimized for modern agentic workflows including Claude Code and Cursor.

**Source:** [hookdeck/webhook-skills/scripts/skill-generator/prompts/generate-skill.md](https://github.com/hookdeck/webhook-skills/blob/da37fc751d55f042ca4eaacb48b0c37ae54b66e0/scripts/skill-generator/prompts/generate-skill.md) · 73★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
Create a complete webhook skill for {{PROVIDER}} following the AGENTS.md specification in this repository.

## Research Phase (CRITICAL - Do This First)

{{DOCS_SECTION}}

**You MUST research and verify the following from official documentation before writing any code:**

### 1. Signature Verification
- What is the **exact header name(s)**? (e.g., `X-Provider-Signature`, `webhook-signature`)
- What algorithm is used? (HMAC-SHA256, ECDSA, etc.)
- What is signed? (raw body, `timestamp.body`, `msgId.timestamp.body`, etc.)
- Does it use Standard Webhooks? (headers: `webhook-id`, `webhook-timestamp`, `webhook-signature`)

### 2. Event Names (VERIFY FROM OFFICIAL DOCS)
- List the **exact** event type strings from the provider's documentation
- Do NOT guess event names - they must match exactly (e.g., `spam report` vs `spam_report` vs `spamreport`)
- Common mistakes: `completed` vs `succeeded`, underscores vs spaces vs dots

### 3. Authentication Method
- API key in header?
- Basic Auth (username:password)?
- OAuth?
- IP allowlist?

## Creation Phase

Read the AGENTS.md file in this repository to understand the full skill creation checklist.

**CRITICAL: You MUST create ALL of the followi
```

</details>
