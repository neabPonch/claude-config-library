---
name: gavdalf__total-recall
source: https://github.com/gavdalf/total-recall/blob/437ab3656ecdf52c7ed0c3ee63a3cdae68d5b90f/SKILL.md
repo: gavdalf/total-recall
kind: skill
stars: 264
last_pushed: 2026-04-01T13:34:49Z
license: mit
score: 9
domains: [agents-ai, cli-tools, memory-management]
tags: [autonomous-memory, context-compression, background-process]
curated: 2026-06-14
curated_by: config-scout
---

# gavdalf/total-recall — skill

**Why it's worth keeping:** The multi-layer architecture (Observer/Reflector/Recovery) provides sophisticated information density management; the use of inotify for reactive triggers and MD5 hashing for deduplication are excellent engineering patterns.

**Summary:** An autonomous background memory system that compresses and consolidates agent session transcripts into a structured observation log to manage context windows.

**Source credibility:** Strong reputation with 264 stars and very recent updates.

**Recency:** Highly relevant to modern agentic workflow constraints regarding context window limits.

**Source:** [gavdalf/total-recall/SKILL.md](https://github.com/gavdalf/total-recall/blob/437ab3656ecdf52c7ed0c3ee63a3cdae68d5b90f/SKILL.md) · 264★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: total-recall
description: "The only memory skill that watches on its own. No database. No vectors. No manual saves. Just an LLM observer that compresses your conversations into prioritised notes, consolidates when they grow, and recovers anything missed. Five layers of redundancy, zero maintenance. ~$0.00/month (using free-tier models). While other memory skills ask you to remember to remember, this one just pays attention."
metadata:
  openclaw:
    emoji: "🧠"
    requires:
      bins: ["jq", "curl"]
    env:
      - key: OPENROUTER_API_KEY
        label: "OpenRouter API key (for LLM calls)"
        required: true
    config:
      memorySearch:
        description: "Enable memory search on observations.md for cross-session recall"
---

# Total Recall — Autonomous Agent Memory

**The only memory skill that watches on its own.**

No database. No vectors. No manual saves. Just an LLM observer that compresses your conversations into prioritised notes, consolidates when they grow, and recovers anything missed. Five layers of redundancy, zero maintenance. ~$0.00/month (using free-tier models).

While other memory skills ask you to remember to remember, this one just pays atte
```

</details>
