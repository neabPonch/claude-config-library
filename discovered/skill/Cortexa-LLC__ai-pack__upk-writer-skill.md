---
name: Cortexa-LLC__ai-pack__upk-writer-skill
source: https://github.com/Cortexa-LLC/ai-pack/blob/b03b7aa707f0e1e0adf1c3c180c7e5dde25ec53c/skills/upk_writer.skill.md
repo: Cortexa-LLC/ai-pack
kind: skill
stars: 0
last_pushed: 2026-06-11T23:43:32Z
license: mit
score: 9
domains: [agents-ai, knowledge-management, cli-tools]
tags: [mcp, meta-learning, personal-knowledge]
curated: 2026-06-16
curated_by: config-scout
---

# Cortexa-LLC/ai-pack — skill

**Why it's worth keeping:** The use of 'Good vs Poor' examples provides high-quality few-shot instructions, and the emphasis on incremental write-back solves the problem of losing context during task timeouts.

**Summary:** Provides a structured framework for an agent to extract and store cross-project insights and decision rationales. It implements a distinction between project-specific data and universal 'personal knowledge'.

**Source credibility:** Low GitHub social proof (0 stars), but the technical sophistication suggests a highly capable author.

**Recency:** 

**Source:** [Cortexa-LLC/ai-pack/skills/upk_writer.skill.md](https://github.com/Cortexa-LLC/ai-pack/blob/b03b7aa707f0e1e0adf1c3c180c7e5dde25ec53c/skills/upk_writer.skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Personal Knowledge Writer (UPK)
<!-- skills/upk_writer.skill.md -->

**Version:** 1.0
**InjectAt:** role_context
**Slot:** 16
**Tools:** mcp__upk__add_learning, mcp__upk__add_conversation
**Gates:** knowledge-first
**MaxExtraTokens:** 5000
**Optional:** true

---

## Personal Knowledge — Record What You Learn

When you discover something meaningful during a task, **record it to personal knowledge immediately**. Future agents (and future you) across ALL projects will benefit from these learnings.

### ⚠️ MANDATORY: Write Back Findings

**REQUIRED operations after learning:**
- ✅ MUST record cross-project insights with `upk__add_learning`
- ✅ MUST record important conversations with `upk__add_conversation`
- ✅ MUST write incrementally (don't wait until task completes)

This is enforced by the **[Knowledge-First Gate](../gates/15-knowledge-first.md)**.

---

## What to Record

### Cross-Project Learnings

| Discovery | How to Record | Example |
|-----------|---------------|---------|
| Design pattern that worked well | `upk__add_learning` | "Circuit breaker pattern in Go: use hystrix-go, set timeout to 5s" |
| Performance optimization discovered | `upk__add_learning` | "Redis connec
```

</details>
