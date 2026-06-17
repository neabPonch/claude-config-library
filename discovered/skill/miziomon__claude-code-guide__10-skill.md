---
name: miziomon__claude-code-guide__10-skill
source: https://github.com/miziomon/claude-code-guide/blob/b6ce14316d0ab1526dcbbc0e883a733f4be7b324/src/it/10-skill.md
repo: miziomon/claude-code-guide
kind: skill
stars: 2
last_pushed: 2026-05-05T19:02:49Z
license: cc0-1.0
score: 9
domains: [agents-ai, cli-tools]
tags: [skill-template, automation, meta-programming]
curated: 2026-06-15
curated_by: config-scout
---

# miziomon/claude-code-guide — skill

**Why it's worth keeping:** Introduces the high-value concept of 'progressive disclosure' to prevent context bloat and provides a repeatable template for project conventions and patterns.

**Summary:** A technical specification for creating Claude Code 'Skills' using SKILL.md files. It details how to use specific frontmatter and description-based triggers to automate agent behavior.

**Source credibility:** High-quality, structured documentation that mirrors professional technical manuals.

**Recency:** Extremely current (dated 2026), specifically targeting advanced agentic workflows.

**Source:** [miziomon/claude-code-guide/src/it/10-skill.md](https://github.com/miziomon/claude-code-guide/blob/b6ce14316d0ab1526dcbbc0e883a733f4be7b324/src/it/10-skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Guida Pratica a Claude Code CLI

> **Versione 4.30 — maggio 2026** — verificata su Claude Code v2.1.123
> Licenza [Creative Commons BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

> ← [9. Sicurezza, permessi e guardrail](09-sicurezza.md) | [Index](README.md) | [11. MCP](11-mcp.md) →

---

## 10. Skill: il meccanismo di estensione

Le Skill sono "playbook" specializzati che Claude può consultare automaticamente quando rileva che un certo tipo di task è in gioco. **Importante**: a differenza degli slash command, **le Skill non si invocano con un comando**. Si attivano automaticamente in base alla loro `description`.

### 10.1 Come funziona una Skill

Una Skill è una cartella con un file `SKILL.md` strutturato così:

```markdown
---
name: wordpress-block-builder
description: "Use this skill when building or modifying WordPress
Gutenberg blocks. Triggers on: block.json, @wordpress/scripts,
JSX files in WordPress plugins, Edit/Save components."
---

# WordPress Block Builder

## Convenzioni del progetto
- Usa sempre @wordpress/scripts per il build
- Ogni blocco deve avere block.json, edit.js, save.js, style.scss
- Attributi devono essere tipizzati in block.json

## Patter
```

</details>
