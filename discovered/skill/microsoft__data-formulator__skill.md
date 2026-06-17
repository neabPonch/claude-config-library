---
name: microsoft__data-formulator__skill
source: https://github.com/microsoft/data-formulator/blob/00d0f5e1655e2a5bb02fda289f73960bbac62027/.cursor/skills/language-injection/SKILL.md
repo: microsoft/data-formulator
kind: skill
stars: 15826
last_pushed: 2026-06-12T23:03:26Z
license: mit
score: 9
domains: [agents-ai, i18n, software-architecture]
tags: [prompt-engineering, localization, standardization]
curated: 2026-06-15
curated_by: config-scout
---

# microsoft/data-formulator — skill

**Why it's worth keeping:** It provides specific anti-patterns to avoid technical debt and uses a dual-mode (full vs compact) injection strategy tailored for different agent behaviors.

**Summary:** Establishes a rigorous protocol for injecting language instructions into LLM system prompts and synchronizing backend-to-frontend localization via message codes.

**Source credibility:** High; part of a high-star Microsoft repository used for data visualization.

**Recency:** Current; follows modern best practices for AI agent instruction management.

**Source:** [microsoft/data-formulator/.cursor/skills/language-injection/SKILL.md](https://github.com/microsoft/data-formulator/blob/00d0f5e1655e2a5bb02fda289f73960bbac62027/.cursor/skills/language-injection/SKILL.md) · 15826★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: language-injection
description: LLM Agent 多语言注入规范。在修改 Agent 提示词、添加新的 Agent 端点、处理用户可见的后端消息（message_code）时使用。
---

# Language Injection for Agent Prompts

Authoritative developer guide: `docs/dev-guides/6-i18n-language-injection.md`.

> **Prerequisites**: Read `docs/dev-guides/6-i18n-language-injection.md` before changing Agent prompts, Agent routes, backend user-visible messages, or frontend i18n strings.
> If your work introduces new language injection patterns or conventions, update this file and related dev-guides accordingly.

## Architecture

```
Frontend i18n.language  →  Accept-Language header  →  get_language_instruction()
                                                           │
                                                   build_language_instruction()
                                                   (agents/agent_language.py)
                                                           │
                                              ┌────────────┴────────────┐
                                              ▼                         ▼
                                        mode="full"               mode="compact"
                                    (text-h
```

</details>
