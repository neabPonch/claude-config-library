---
name: eze-is__ai-partner-chat
source: https://github.com/eze-is/ai-partner-chat/blob/1170b66b4b9b0194fb45d622cdd7bcd575c05df1/SKILL.md
repo: eze-is/ai-partner-chat
kind: skill
stars: 216
last_pushed: 2026-01-15T02:47:51Z
license: unknown
score: 8
domains: [agents-ai, cli-tools, knowledge-management]
tags: [rag, persona, vector-db, personal-intelligence]
curated: 2026-06-16
curated_by: config-scout
---

# eze-is/ai-partner-chat — skill

**Why it's worth keeping:** The 'agentic chunking' concept—where the agent generates custom code to parse specific note structures rather than using static rules—is a highly advanced and transferable pattern for local data ingestion.

**Summary:** A local RAG framework that combines user/AI personas with a vector database of markdown notes to provide deep, personalized context awareness.

**Source credibility:** Moderate popularity with 216 stars, suggesting a proven community interest.

**Recency:** Highly relevant; updated within the last 5 months to align with current agentic workflows.

**Source:** [eze-is/ai-partner-chat/SKILL.md](https://github.com/eze-is/ai-partner-chat/blob/1170b66b4b9b0194fb45d622cdd7bcd575c05df1/SKILL.md) · 216★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ai-partner-chat
description: 基于用户画像和向量化笔记提供个性化对话。当用户需要个性化交流、上下文感知的回应，或希望 AI 记住并引用其之前的想法和笔记时使用。
---

# AI Partner Chat

## Overview

Provide personalized, context-aware conversations by integrating user persona, AI persona, and vectorized personal notes. This skill enables AI to remember and reference the user's previous thoughts, preferences, and knowledge base, creating a more coherent and personalized interaction experience.

## Prerequisites

Before first use, complete these steps in order:

1. **Create directory structure**
   ```bash
   mkdir -p config notes vector_db scripts
   ```

2. **Set up Python environment**
   ```bash
   python3 -m venv venv
   ./venv/bin/pip install -r .claude/skills/ai-partner-chat/scripts/requirements.txt
   ```
   Note: First run will download embedding model (~4.3GB)

3. **Generate persona templates**
   Copy from `.claude/skills/ai-partner-chat/assets/` to `config/`:
   - `user-persona-template.md` → `config/user-persona.md`
   - `ai-persona-template.md` → `config/ai-persona.md`

4. **User adds notes**
   Place markdown notes in `notes/` directory (any format/structure)

5. **Initialize vector database** (see section 1.2 below)

Now pr
```

</details>
