---
name: SnailSploit__Claude-Red__skill
source: https://github.com/SnailSploit/Claude-Red/blob/aeb41eca7088a703c3a35fbcba3086d4a6c1aa4e/Skills/web/offensive-idor/SKILL.md
repo: SnailSploit/Claude-Red
kind: skill
stars: 2322
last_pushed: 2026-05-08T16:05:21Z
license: mit
score: 9
domains: [security, backend-api, web-pentesting]
tags: [security, offensive-security, idor, bug-bounty]
curated: 2026-06-16
curated_by: config-scout
---

# SnailSploit/Claude-Red — skill

**Why it's worth keeping:** The use of Mermaid diagrams for logical flow and highly specific parameter manipulation techniques (like JSON object wrapping and array-based access) makes it immediately actionable for an agent.

**Summary:** Provides a professional pentesting methodology for identifying IDOR vulnerabilities using structured logic and detailed attack patterns.

**Source credibility:** High; the repository is a specialized, high-star resource specifically designed for offensive security skills.

**Recency:** Current; the structured instruction format is optimized for modern agentic workflows like Claude Code.

**Source:** [SnailSploit/Claude-Red/Skills/web/offensive-idor/SKILL.md](https://github.com/SnailSploit/Claude-Red/blob/aeb41eca7088a703c3a35fbcba3086d4a6c1aa4e/Skills/web/offensive-idor/SKILL.md) · 2322★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SKILL: Insecure Direct Object References (IDOR)

## Metadata
- **Skill Name**: idor
- **Folder**: offensive-idor
- **Source**: https://github.com/SnailSploit/offensive-checklist/blob/main/idor.md

## Description
IDOR (Insecure Direct Object Reference) testing checklist: object ID enumeration, horizontal/vertical privilege escalation, GUID predictability, indirect references via hashes, chained IDOR, and API endpoint IDOR. Use for web app pentests and bug bounty IDOR discovery.

## Trigger Phrases
Use this skill when the conversation involves any of:
`IDOR, insecure direct object reference, horizontal privilege escalation, vertical privilege escalation, object enumeration, GUID, API IDOR, mass assignment, broken access control`

## Instructions for Claude

When this skill is active:
1. Load and apply the full methodology below as your operational checklist
2. Follow steps in order unless the user specifies otherwise
3. For each technique, consider applicability to the current target/context
4. Track which checklist items have been completed
5. Suggest next steps based on findings

---

## Full Methodology

# Insecure Direct Object References (IDOR)

## Shortcut

```mermaid
flowcha
```

</details>
