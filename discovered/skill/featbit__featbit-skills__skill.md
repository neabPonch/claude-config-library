---
name: featbit__featbit-skills__skill
source: https://github.com/featbit/featbit-skills/blob/008b7a697b461db4e353cb1d264617628064d56c/skills/featbit-documentation/SKILL.md
repo: featbit/featbit-skills
kind: skill
stars: 11
last_pushed: 2026-04-28T07:03:45Z
license: mit
score: 7
domains: [platform-ops, documentation-automation]
tags: [router, knowledge-index, fallback-strategy]
curated: 2026-06-16
curated_by: config-scout
---

# featbit/featbit-skills — skill

**Why it's worth keeping:** It utilizes a 'Map-to-Action' pattern where the skill provides a high-level index rather than raw content, allowing the agent to select highly relevant URLs for targeted information retrieval.

**Summary:** A fallback documentation router that provides a categorized taxonomy of URLs to guide an agent toward specific official resources.

**Source credibility:** High; written by the actual FeatBit team/organization.

**Recency:** Current; follows modern agentic orchestration patterns used in tool-calling environments.

**Source:** [featbit/featbit-skills/skills/featbit-documentation/SKILL.md](https://github.com/featbit/featbit-skills/blob/008b7a697b461db4e353cb1d264617628064d56c/skills/featbit-documentation/SKILL.md) · 11★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: featbit-documentation
description: FeatBit documentation router that provides likely relevant docs.featbit.co URLs when other FeatBit skills cannot fully answer. Use when user asks about FeatBit features, concepts, deployment, SDKs, API, integrations, or architecture and the response should point to official documentation for deeper detail. Do not use when another FeatBit skill already provides a complete answer.
license: MIT
metadata:
  author: FeatBit
  version: 2.0.0
  category: platform
---

# FeatBit Documentation Router

This skill is a **fallback** for FeatBit questions. Use it **only after** other FeatBit skills do not provide a complete answer. Its job is to return a short list of **likely relevant documentation URLs** so the agent can open those pages and extract the final details.

## When to Use This Skill

Activate this skill when:
- A FeatBit question is not fully answered by more specific FeatBit skills.
- The request requires authoritative details from FeatBit docs.
- The best next step is to point the agent to official documentation URLs.

Do **not** use this skill when another FeatBit skill already provides a full answer.

## Output Rules (Critical)

1.
```

</details>
