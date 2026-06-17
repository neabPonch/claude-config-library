---
name: titanwings__colleague-skill
source: https://github.com/titanwings/colleague-skill/blob/47039d08fcf0330794caea14efdb5e183348f7bb/SKILL.md
repo: titanwings/colleague-skill
kind: skill
stars: 19378
last_pushed: 2026-06-01T08:03:05Z
license: mit
score: 9
domains: [agents-ai, data-extraction, automation, persona-engineering]
tags: [meta-skill, character-distillation, api-orchestration, enterprise-tools]
curated: 2026-06-14
curated_by: config-scout
---

# titanwings/colleague-skill — skill

**Why it's worth keeping:** It provides high-fidelity orchestration for complex API/OAuth flows and demonstrates how an agent can use Python scripts to overcome platform-specific data retrieval limitations.

**Summary:** A meta-skill engine designed to 'distill' individuals into reusable character profiles by aggregating data from platforms like Feishu, DingTalk, or local files.

**Source credibility:** Extremely high; 19k+ stars indicates significant community adoption and proven utility.

**Recency:** Highly current, utilizing modern enterprise integration patterns (Feishu/DingTalk).

**Source:** [titanwings/colleague-skill/SKILL.md](https://github.com/titanwings/colleague-skill/blob/47039d08fcf0330794caea14efdb5e183348f7bb/SKILL.md) · 19378★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: dot-skill
description: "Unified meta-skill engine for distilling colleague, relationship, or celebrity characters into reusable Skills. | 统一的 meta-skill 引擎，把 colleague、relationship、celebrity 三类对象蒸馏成可复用 Skill。"
argument-hint: "[character] [name-or-slug]"
version: "1.0.0"
user-invocable: true
allowed-tools: Read, Write, Edit, Bash
---

> **Language / 语言**: This skill supports both English and Chinese. Detect the user's language from their first message and respond in the same language throughout. Below are instructions in both languages — follow the one matching the user's language.
>
> 本 Skill 支持中英文。根据用户第一条消息的语言，全程使用同一语言回复。下方提供了两种语言的指令，按用户语言选择对应版本执行。

> **Execution Root / 执行根目录**: Run all `Bash` commands from the directory that contains this `SKILL.md`. All `tools/...` and `prompts/...` paths below are relative to the skill root.
>
> **Critical rule / 关键规则**: Do **not** prepend commands with guessed host-specific paths such as `cd ~/.hermes/...`, `cd ~/.claude/...`, `cd ~/.openclaw/...`, `cd ~/.codex/...`, or hard-coded `/Users/.../dot-skill` paths. The current working directory is already the correct skill root. Run `python3 tools/...` directly.
>
> 所有 `Bash` 命令都必须在当前 `SK
```

</details>
