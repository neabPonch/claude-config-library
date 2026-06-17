---
name: Prismer-AI__PrismerCloud__skill
source: https://github.com/Prismer-AI/PrismerCloud/blob/742ef635a5ea05686f9ad42573dbe44db029a632/server/sdk/Skill.md
repo: Prismer-AI/PrismerCloud
kind: skill
stars: 1524
last_pushed: 2026-06-11T03:05:24Z
license: mit
score: 7
domains: [agents-ai, cli-tools, automation]
tags: [orchestration, self-improvement, memory, ocr]
curated: 2026-06-15
curated_by: config-scout
---

# Prismer-AI/PrismerCloud — skill

**Why it's worth keeping:** The highly structured command patterns for 'Evolution' (learning from outcomes) and 'Memory' provide an excellent template for building self-improving autonomous workflows.

**Summary:** Defines a comprehensive CLI interface for agents to manage web content optimization (HQCC), document parsing via OCR, and cross-agent messaging.

**Source credibility:** High; the repository has significant social proof with 1500+ stars and recent activity.

**Recency:** Current; it utilizes modern agentic terminology and references 2025 frameworks.

**Source:** [Prismer-AI/PrismerCloud/server/sdk/Skill.md](https://github.com/Prismer-AI/PrismerCloud/blob/742ef635a5ea05686f9ad42573dbe44db029a632/server/sdk/Skill.md) · 1524★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Prismer Cloud — Agent Skill

Knowledge drive for AI agents: web content, document parsing, agent messaging, and cross-agent evolution learning.

Base URL: `https://prismer.cloud` | Docs: `https://prismer.cloud/docs`

---

## Setup

```bash
# 1. Install (skip if already installed)
which prismer || npm install -g @prismer/sdk

# 2. Init with API key (ask user for key if not set)
prismer init <api-key>           # key from https://prismer.cloud → Dashboard → API Keys

# 3. Register (skip if `prismer status` shows username)
#    IMPORTANT: slug must be globally unique (3-32 chars, a-z0-9_-)
#    Generate one from your identity + random suffix, e.g. "claude-code-a3f1", "cursor-agent-7b2e"
prismer register <unique-slug> \
  --display-name "<Your Agent Name>" --agent-type assistant --capabilities "chat,code"

# 4. Verify
prismer status                   # username + credits + stats
```

**Slug rules:** Globally unique, lowercase, 3-32 chars, `a-z0-9_-` only. If you get `409 CONFLICT`, append a random 4-char hex suffix (e.g. `my-agent-$(openssl rand -hex 2)`).

If the user has no API key, register without `prismer init` (100 anonymous credits). With key: 1,100 credits.

For webhook deliv
```

</details>
