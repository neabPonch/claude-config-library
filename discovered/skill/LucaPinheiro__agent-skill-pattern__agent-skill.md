---
name: LucaPinheiro__agent-skill-pattern__agent-skill
source: https://github.com/LucaPinheiro/agent-skill-pattern/blob/5eb496dcfa5e963696cba7937eb03bfa55e53d49/agent-skill.md
repo: LucaPinheiro/agent-skill-pattern
kind: skill
stars: 0
last_pushed: 2026-05-12T18:44:13Z
license: unknown
score: 8
domains: [agents-ai, architecture]
tags: [progressive-disclosure, skill-pattern, context-management]
curated: 2026-06-16
curated_by: config-scout
---

# LucaPinheiro/agent-skill-pattern — skill

**Why it's worth keeping:** Provides a high-level architectural distinction between 'tools' (actions) and 'skills' (procedural logic), using on-demand loading to keep the system prompt lean.

**Summary:** Defines a 'Progressive Disclosure' pattern for agentic skills to prevent context window saturation and tool-call explosion.

**Source credibility:** Low social proof (0 stars), but demonstrates professional-grade architectural thinking/ADRs.

**Recency:** Highly current; aligns with modern agentic orchestration trends from 2024/2025.

**Source:** [LucaPinheiro/agent-skill-pattern/agent-skill.md](https://github.com/LucaPinheiro/agent-skill-pattern/blob/5eb496dcfa5e963696cba7937eb03bfa55e53d49/agent-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Agent Skills Pattern — Guia de Implementação para Template Agentic em LangGraph

> **Escopo deste documento.** Esta referência descreve o padrão **Agent Skills** e detalha como incorporá-lo a um **template** de construção de agentes em LangGraph. Não estamos descrevendo a plataforma agentic builder como um todo — apenas o template que será o ponto de partida para qualquer novo agente construído sobre ela.
>
> **Audiência.** Engenheiros e arquitetos de IA que vão consumir o template, customizá-lo e estender com novas skills. Pressupõe familiaridade com LangGraph (StateGraph, nodes, edges, middleware) e com o conceito básico de tool calling.

---

## Sumário

1. [Por que Skills (e não só prompts ou só tools)](#1-por-que-skills-e-não-só-prompts-ou-só-tools)
2. [Conceitos centrais](#2-conceitos-centrais)
   - [2.4 Decisão arquitetural — tool `load_skill` vs filesystem-native (ADR)](#24-decisão-arquitetural--tool-load_skill-vs-filesystem-native-adr)
3. [Anatomia de uma Skill](#3-anatomia-de-uma-skill)
4. [O padrão AKU — Atomic Knowledge Unit](#4-o-padrão-aku--atomic-knowledge-unit)
5. [Estrutura de diretórios do template](#5-estrutura-de-diretórios-do-template)
6. [Implementação em La
```

</details>
